# Instructions to Restart Django Server and Clear Template Cache

If you have updated your Django templates but still see errors like TemplateSyntaxError related to template tag libraries, it is likely due to cached templates or the server not being restarted.

Follow these steps to ensure your changes take effect:

## Restart Django Development Server

1. Stop the running server by pressing `Ctrl+C` in the terminal where it is running.
2. Start the server again with:

   ```
   python manage.py runserver
   ```

## Clear Template Cache (if applicable)

If you are using any caching mechanism for templates (e.g., cached template loader), clear the cache by:

- Restarting the server (usually sufficient).
- Deleting any cache files or clearing cache storage if configured.

## Verify Virtual Environment

Make sure your virtual environment is activated before running the server:

- On Windows:

  ```
  venv\Scripts\activate
  ```

- On Linux/macOS:

  ```
  source venv/bin/activate
  ```

## Additional Tips

- Ensure your templates load the correct tag library name, e.g., `{% load django_bootstrap5 %}`.
- If you continue to see errors, try clearing your browser cache or use a private/incognito window.

If you need further assistance, feel free to ask.
