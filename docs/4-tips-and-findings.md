# Tips and findings

There are some things that need to be kept in mind during working with WordPress sites:

- Do not name the administrator user `admin`: hacker bots try to crack the credentials directly with this username
- If you want to upload a file or theme and get this error: `he uploaded file exceeds the upload_max_filesize directive in php.ini`, then co to .htaccess, and add this line to the end of the file: `php_value upload_max_filesize 256M`
  - You can check the maximum file size at: `Media/Add new`
