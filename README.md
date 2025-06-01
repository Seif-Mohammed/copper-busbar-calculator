# Copper Busbar Bending Calculator

A professional PyQt6-based application for calculating copper busbar bending dimensions with support for multiple bar configurations.

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![PyQt6](https://img.shields.io/badge/PyQt6-GUI-green.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Features

- **Multiple Shape Support**: L-Shape, U-Shape, and Z-Shape configurations
- **Multiple Bar Calculations**: Calculate dimensions for multiple bars with spacing adjustments
- **Precise Bend Calculations**: Uses K-factor methodology for accurate bend allowances
- **Professional Results Export**: Export detailed calculations to formatted text files
- **Visual Shape Diagrams**: Interactive diagrams showing bend configurations
- **Dark Theme Interface**: Modern copper-themed UI design
- **Secure Authorization**: Password-protected software access

## Supported Shapes

### L-Shape
- Two perpendicular segments with single bend
- Ideal for corner connections

### U-Shape  
- Three segments with two bends forming a U
- Perfect for bypass configurations

### Z-Shape
- Three segments with two opposite bends
- Used for offset connections

## Installation

### Prerequisites
- Python 3.8 or higher
- PyQt6

### Setup
1. Clone the repository:
```bash
git clone https://github.com/yourusername/copper-busbar-calculator.git
cd copper-busbar-calculator
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python BUSBAR_BENDING_V1.py
```

## Usage

### Getting Started
1. Launch the application
2. Enter the authorization passkey when prompted
3. Configure your busbar parameters:
   - Number of bars
   - Spacing between bars
   - Shape type (L, U, or Z)
   - Material dimensions (thickness, width)
   - Bend specifications (radius, angles)
   - Segment lengths

### Calculation Parameters

| Parameter | Description | Range |
|-----------|-------------|-------|
| Number of Bars | Quantity of bars to calculate | 1-100 |
| Spacing | Distance between bars (mm) | 0-500 |
| Thickness | Bar thickness (mm) | 0.1-100 |
| Width | Bar width (mm) | 0.1-1000 |
| Bend Radius | Internal bend radius (mm) | 0.1-100 |
| K-Factor | Neutral axis position factor | 0.01-1.0 |
| Bend Angles | Bending angles (degrees) | 0-180 |

### Output Information
- **Flat Length**: Total material length needed before bending
- **Bend Locations**: Precise positions for bend operations
- **Bend Deductions**: Material allowances for bending
- **Weight Calculations**: Total material weight in grams
- **Individual Bar Dimensions**: Detailed calculations for each bar

## Technical Details

### Bend Calculation Method
The application uses the **neutral axis method** for bend allowance calculations:

```
Bend Allowance = (π/180) × (R + K×T) × A
```

Where:
- R = Bend radius
- K = K-factor (typically 0.4 for copper)
- T = Material thickness  
- A = Bend angle in degrees

### Material Properties
- **Material**: Copper
- **Density**: 8.96 g/cm³
- **Default K-Factor**: 0.4 (optimized for copper)

## File Structure

```
copper-busbar-calculator/
│
├── BUSBAR_BENDING_V1.py      # Main application file
├── requirements.txt           # Python dependencies
├── README.md                 # Project documentation
├── LICENSE                   # Software license
├── .gitignore               # Git ignore rules
└── screenshots/             # Application screenshots
    ├── main_interface.png
    ├── calculation_results.png
    └── shape_diagrams.png
```

## Export Features

The application provides comprehensive export functionality:
- **Formatted Text Reports**: Professional calculation reports
- **Timestamped Files**: Automatic date/time stamping
- **Engineer Attribution**: Includes engineer information and contact details
- **Detailed Breakdowns**: Complete calculation methodology and results

## Authorization

This software includes a security system requiring authorized access. Contact the developer for access credentials:

**Engineer**: Seif Mohamed  
**Email**: seifmohamed606@gmail.com

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Setup
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

**Engineer**: Seif Mohamed  
**Email**: seifmohamed606@gmail.com  
**Project Link**: https://github.com/yourusername/copper-busbar-calculator

## Acknowledgments

- PyQt6 development team for the excellent GUI framework
- Copper industry standards for bend calculation methodologies
- Engineering community for feedback and testing

---

*Professional engineering software for copper busbar fabrication and installation.*
