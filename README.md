# ShopMind — E-commerce Web Application

ShopMind is a PHP/MySQL e-commerce team project with a customer storefront, vendor pages, and an admin dashboard.

## Stack
- PHP and MySQL/MariaDB
- HTML, CSS, JavaScript
- Bootstrap, jQuery, Font Awesome, Chart.js, DataTables (bundled under `vendor/`)

## Run locally (XAMPP)
1. Copy the repository folder into `C:\xampp\htdocs\`.
2. Start Apache and MySQL from XAMPP.
3. Create/import the `store` database and required tables. The repository currently includes `SQL/ban_users_migration.sql`; it is a migration, not a complete database dump.
4. Copy `fun/db_config.example.php` to `fun/db_config.local.php` and set your local database credentials. The local config is ignored by Git.
5. Open the storefront at `http://localhost/ShopMind-main_dashbord/ShopMind-main/ShopMind-main/frontend/index.php` (adjust the URL to match your folder name).

## Database configuration
`fun/db_connection.php` loads `fun/db_config.local.php` when present. Alternatively, set `SHOPMIND_DB_HOST`, `SHOPMIND_DB_USER`, `SHOPMIND_DB_PASSWORD`, and `SHOPMIND_DB_NAME` in your PHP environment. Never commit real credentials or production database dumps.

## Notes
- Product images and frontend assets are included.
- `vendor/` contains runtime libraries used by the pages; keep it when deploying this project as-is.
- This is a student/team project. Features and database setup may require configuration for your environment.
