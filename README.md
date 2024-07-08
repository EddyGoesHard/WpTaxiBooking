# Taxi Booking Plugin

This plugin allows users to book taxis through a WordPress website using the Mollie API for payment processing.

## Features

- Book a taxi by filling out a form.
- Validate user input for name, email, pickup location, dropoff location, and pickup date.
- Store booking information securely in WordPress database.
- Send email confirmation to the customer after successful booking.
- Integrate with Mollie API for payment processing.

## Installation

1. Clone the repository or download the ZIP file and extract it into your WordPress plugins directory (`wp-content/plugins/`).
2. Activate the "Taxi Booking Plugin" through the 'Plugins' menu in WordPress.
3. Configure plugin settings via the "Book A Taxi" menu in the WordPress admin dashboard.

## Functions

Sure, here's a list of functions commonly used in a Taxi Booking Plugin for WordPress:

1. **Main Plugin Functions:**
   - `book_a_taxi_process_booking_form()`: Validates and processes the taxi booking form data.
   - `book_a_taxi_enqueue_scripts()`: Enqueues CSS and JavaScript files for frontend functionality.
   - `book_a_taxi_load_textdomain()`: Loads the plugin's text domain for localization.
   - `book_a_taxi_activation_hook()`: Runs when the plugin is activated, performs initialization tasks.
   - `book_a_taxi_deactivation_hook()`: Runs when the plugin is deactivated, cleans up or saves data.

2. **Form Handling Functions:**
   - `book_a_taxi_process_booking_form()`: Validates and processes the booking form data.
   - `book_a_taxi_display_booking_form()`: Displays the booking form using a shortcode or function call.
   - `book_a_taxi_validate_booking_data()`: Validates input fields like name, email, locations, and dates.

3. **Database Interaction Functions:**
   - `book_a_taxi_save_booking_to_database()`: Saves validated booking data to the WordPress database.
   - `book_a_taxi_get_booking_details()`: Retrieves booking details from the database based on booking ID.

4. **Email Functions:**
   - `book_a_taxi_send_booking_confirmation_email()`: Sends an email confirmation to the customer after successful booking.
   - `book_a_taxi_send_admin_notification_email()`: Sends an email notification to the admin about a new booking.

5. **Payment Processing Functions:**
   - `book_a_taxi_process_payment()`: Processes payments using the Mollie API or other payment gateways.
   - `book_a_taxi_handle_payment_webhook()`: Handles webhook notifications from payment processors.
   - `book_a_taxi_display_payment_status()`: Displays payment status to users after completing a payment.

6. **Settings and Admin Functions:**
   - `book_a_taxi_register_settings()`: Registers plugin settings and options in the WordPress admin.
   - `book_a_taxi_render_options_page()`: Renders the plugin's settings page in the WordPress admin dashboard.
   - `book_a_taxi_admin_enqueue_scripts()`: Enqueues CSS and JavaScript files for the admin dashboard.

7. **Utility Functions:**
   - `book_a_taxi_generate_booking_id()`: Generates a unique booking ID for each booking.
   - `book_a_taxi_format_date()`: Formats dates and times for display or storage.
   - `book_a_taxi_validate_email_address()`: Validates email addresses using WordPress functions or PHP filters.

8. **Localization and Internationalization Functions:**
   - `book_a_taxi_load_textdomain()`: Loads the plugin's text domain for translation.
   - `book_a_taxi_translate_text()`: Translates text strings into different languages using WordPress localization functions.

9. **Security Functions:**
   - `book_a_taxi_validate_input_data()`: Validates and sanitizes user input to prevent security vulnerabilities.
   - `book_a_taxi_secure_admin_pages()`: Implements security measures for admin pages, such as nonce verification.

10. **Debugging and Logging Functions:**
    - `book_a_taxi_log_error()`: Logs errors and debug information for troubleshooting.
    - `book_a_taxi_debug_mode_enabled()`: Checks if debug mode is enabled and logs additional information.

These functions cover various aspects of a Taxi Booking Plugin, from form handling and database interaction to email notifications, payment processing, settings management, and security considerations. Depending on your specific plugin requirements, you may implement additional functions or customize existing ones further.

## Usage

1. Use the `[taxi_booking_form]` shortcode to display the booking form on any page or post.
2. Users fill out the form with their details and confirm the booking.
3. Upon successful submission, users receive an email confirmation, and the booking details are stored in the database.

## Configuration

- **Mollie API Integration:** Obtain your Mollie API key and enter it in the plugin settings to enable payment processing.
- **Email Notifications:** Customize the email template for booking confirmations in the plugin settings.

## Directory structure
```
Taxi-Booking-Plugin/
├── book-a-taxi.php
├── book-a-taxi-functions.php
├── book-a-taxi-admin.php
├── book-a-taxi-scripts.php
├── languages/
│   └── book-a-taxi-en_US.mo
│   └── book-a-taxi-en_US.po
├── payments/
│   ├── book-a-taxi-payment.php
│   ├── book-a-taxi-webhook.php
│   └── book-a-taxi-payment-success.php
├── css/
│   └── book-a-taxi.css
├── js/
│   └── book-a-taxi.js
├── inc/
│   └── class-wp-bootstrap-navwalker.php
├── vendor/
│   └── mollie/
│       └── mollie-api-php/
│           ├── src/
│           ├── tests/
│           ├── composer.json
│           └── README.md
├── README.md
├── LICENSE
└── index.php
```
## Contributing

Contributions are welcome! If you have any feature requests, suggestions, or bug reports, please [open an issue](https://github.com/your-repo/issues).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
