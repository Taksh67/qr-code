# QR Code Generation & Scanning System

A full-stack MERN application for generating, scanning, and managing QR codes.

## Features

- Generate QR codes from text or URLs
- Scan QR codes using device camera
- View history of generated QR codes
- Download QR codes as images
- Copy QR code URLs to clipboard
- Share QR codes via email
- Filter QR codes by date range
- Paginated QR code history

## Tech Stack

- **Frontend:** React (Vite) + Material-UI
- **Backend:** Node.js + Express
- **Database:** MongoDB
- **QR Code Generation:** qrcode
- **QR Code Scanning:** react-qr-reader
- **Email:** Nodemailer

## Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd qr-code-system
   ```

2. Install backend dependencies:
   ```bash
   cd server
   npm install
   ```

3. Create a `.env` file in the server directory:
   ```
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/qr-code-system
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASS=your_email_app_password
   ```

4. Install frontend dependencies:
   ```bash
   cd ../client
   npm install
   ```

5. Start the backend server:
   ```bash
   cd ../server
   npm run dev
   ```

6. Start the frontend development server:
   ```bash
   cd ../client
   npm run dev
   ```

7. Open your browser and navigate to `http://localhost:3000`

## Usage

1. Generate QR codes by entering text or URLs
2. View your generated QR codes in the dashboard
3. Use the scanner to scan QR codes with your device's camera
4. Download, share, or delete QR codes as needed
5. Filter QR codes by date range
6. Navigate through pages of QR code history

## API Endpoints

### QR Codes
- `POST /api/qrcodes` - Generate a new QR code
- `GET /api/qrcodes` - Get all QR codes (with pagination & filters)
- `DELETE /api/qrcodes/:id` - Delete a QR code
- `POST /api/qrcodes/share` - Share QR code via email

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 