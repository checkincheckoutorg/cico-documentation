# Database Contracts

# Account
## Table Schema
Columns:
- unique_id, string, unique
- id, int, primary key, auto increment
- first_name, string
- last_name, string
- email, string
- age, int
- admin_status, bool
- encrypted_password, string
- salt, string
- created_at, datetime
- updated_at, datetime

# Book
## Table Schema
Columns:
- id, int, primary key, auto increment
- isbn, string, unique
- title, string
- author, string
- genre, string
- stock, int
- front_cover, string
- book_type, string

# BookHistory
## Table Schema
Columns:
- id, int, primary key, auto increment
- book_id, int, auto increment, unique
- account_id, int, auto increment, unique
- book_action, string
- action_time, datetime

# Endpoints
