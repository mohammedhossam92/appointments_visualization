# Appointments Visualization System (نظام تصور المواعيد)

A dental clinic appointment management and visualization system with an Arabic interface.

## Features

- 📅 Interactive calendar view (monthly, weekly, daily)
- 📊 Statistical dashboard for appointment tracking
- 📁 Support for Excel (.xlsx, .xls) and CSV file imports
- 🌐 Right-to-left (RTL) Arabic interface
- 🎨 Modern dark mode design

## Usage

1. Open `index.html` in a web browser
2. Click "حمّل ملف Excel أو CSV" to upload an appointment file
3. View appointments on the interactive calendar
4. Click on events to see detailed information

## Supported File Format

The application expects Excel or CSV files with the following Arabic column headers:
- اليوم (Day)
- التاريخ (Date)
- غرفة الكشف (Examination Room)
- من (Start Time)
- حتى (End Time)
- الأسم (Patient Name)
- الإجراء (Procedure)
- الطبيب (Doctor)
- تليفون (Phone)

See `sample_appointments.csv` for an example.

## Browser Compatibility

This application works best with modern web browsers. If you encounter tracking prevention warnings:

1. The application uses CDN-hosted libraries (FullCalendar and SheetJS) with `crossorigin="anonymous"` to prevent tracking issues
2. If libraries fail to load, you'll see a clear error message in Arabic
3. For best results, ensure your browser allows loading resources from CDN providers (jsdelivr.net and cdnjs.cloudflare.com)

### Troubleshooting

If you see the error "⚠️ فشل تحميل مكتبة التقويم":
- Check your internet connection
- Temporarily disable strict tracking prevention in your browser
- Clear browser cache and reload the page
- Ensure your browser/network isn't blocking CDN resources

## Technical Details

- **Frontend**: Pure HTML/CSS/JavaScript (no build process required)
- **Calendar Library**: FullCalendar v6.1.10
- **Excel Parser**: SheetJS (xlsx) v0.18.5
- **Styling**: Custom CSS with RTL support