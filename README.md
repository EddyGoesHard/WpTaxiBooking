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

## Usage

1. Use the `[taxi_booking_form]` shortcode to display the booking form on any page or post.
2. Users fill out the form with their details and confirm the booking.
3. Upon successful submission, users receive an email confirmation, and the booking details are stored in the database.

## Configuration

- **Mollie API Integration:** Obtain your Mollie API key and enter it in the plugin settings to enable payment processing.
- **Email Notifications:** Customize the email template for booking confirmations in the plugin settings.

## Contributing

Contributions are welcome! If you have any feature requests, suggestions, or bug reports, please [open an issue](https://github.com/your-repo/issues).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
