# Fredericksburg City Council - Tactical Intelligence Network Analysis

## 🎯 Overview
An interactive web-based intelligence system for analyzing the Fredericksburg City Council network with a military-grade Palantir/Call of Duty Black Ops inspired interface.

## ✨ Key Features

### Visual Design
- **Tactical Military Interface** - Dark theme with cyan (#00d9ff) and orange (#ff6b00) accent colors
- **Animated Grid Background** - Precision measurement grid with tactical overlay
- **Corner Targeting Brackets** - Military-style corner decorations
- **Scanline Effect** - Sweeping scan animation across the screen
- **Hexagonal Node Design** - Military-grade hexagonal nodes with crosshairs and corner brackets
- **ID Tags** - Each node displays a unique identifier (#001, #002, etc.)

### Interactive Network Visualization
- **11 Council Members & Officials** fully mapped with complete data
- **Color-coded by Role**:
  - Mayor: Orange (#ff6b00)
  - Council Members: Cyan (#00d9ff)
  - City Attorney: Blue (#00a8ff)
  - City Officials: Gold (#ffd000)

### Navigation & Controls
- **Canvas Panning**: 
  - Right-click + drag to pan the view
  - Shift + click + drag to pan the view
- **Zoom**: Mouse wheel/scroll to zoom in/out
- **Node Interaction**:
  - Click nodes to view detailed profiles
  - Drag individual nodes to reposition them
- **Hover Tooltips**: Quick info on mouse hover

### Sorting & Analysis Modes
1. **Chain of Command** - Hierarchical organizational view
2. **Business Connections** - Network web showing business relationships
3. **Family Connections** - Network web showing family relationships
4. **Non-Profit Connections** - Network web showing organizational affiliations
5. **Political Affiliation** - Grouped by political party/spectrum

### Comprehensive Member Profiles
Each node contains detailed information:
- **Official Website** - Direct link to government profile
- **Social Media Links** - Facebook, Twitter/X, LinkedIn (when available)
- **Addresses & Properties**
- **Education** - With links to institutions
- **Political Affiliation & Spectrum**
- **Professional Background**
- **Business Affiliations** - Clickable links to organizations
- **Family Connections**
- **Non-Profit/Organization Memberships** - All with clickable website links
- **Complete Voting Records**
- **Criminal Records**

### Clickable Links
All organizations, schools, businesses, and affiliations are **hyperlinked** to their respective websites for deep-dive research:
- Educational institutions
- Non-profit organizations
- Government agencies
- Business entities
- Social media profiles

### Data Management
- **Export Data** - Download full dataset as JSON
- **Import Data** - Load custom data from .json, .csv, or .txt files
- **Reset View** - Return to default layout
- **Expand/Collapse All** - Quick view management

### Connection Visualization
- **Dashed connection lines** show relationships between nodes
- **Midpoint indicators** mark connection paths
- **Dynamic network mapping** based on selected sort type

## 🎮 Controls Guide

| Action | Method |
|--------|--------|
| Pan Canvas | Right-Click + Drag OR Shift + Drag |
| Zoom | Mouse Wheel / Scroll |
| View Details | Click on Node |
| Move Node | Click + Drag Node |
| Reset View | Click "RESET VIEW" button |
| Close Details Panel | Click X button |

## 📊 Data Structure

Each member includes:
```javascript
{
    id: Number,
    name: String,
    title: String,
    position: String,
    website: String (URL),
    socialMedia: {
        facebook: String (URL),
        twitter: String (URL),
        linkedin: String (URL)
    },
    addresses: String,
    properties: String,
    affiliations: Array (with |URL separators),
    education: String (with |URL separator),
    political: String,
    politicalSpectrum: String,
    voting: Array,
    criminal: String,
    background: String,
    businessConnections: Array,
    familyConnections: Array,
    nonprofitConnections: Array
}
```

## 🔗 Link Format
Organizations and institutions use the format:
```
"Organization Name|https://website.com/"
```

The system automatically converts these to clickable links with hover effects.

## 🎨 Color Scheme
- Primary: Cyan (#00d9ff)
- Secondary: Orange (#ff6b00)
- Background: Deep Navy (#0a0e1a)
- Text: Light Cyan (#a8c5d1)
- Accents: Gold (#ffd000), Blue (#00a8ff)

## 📱 Responsive Design
- Fully responsive for desktop and mobile devices
- Adaptive layout for tablets and smartphones
- Touch-friendly controls for mobile interaction

## 🚀 Performance
- Smooth 60 FPS animations
- Efficient canvas rendering
- Optimized force-directed layout algorithm
- No external dependencies (vanilla JavaScript)

## 🔒 Privacy & Security
- All data is client-side only
- No external data collection
- No tracking or analytics
- Secure HTTPS links to external resources

## 📄 File Information
- **Primary File**: citycouncil.html
- **Size**: Single HTML file with embedded CSS and JavaScript
- **Dependencies**: None (100% self-contained)
- **Browser Compatibility**: Modern browsers (Chrome, Firefox, Edge, Safari)

## 🎯 Use Cases
- City governance research
- Network analysis and visualization
- OSINT (Open Source Intelligence) gathering
- Civic transparency and accountability
- Educational tool for understanding local government
- Connection mapping and relationship discovery

## 🔧 Customization
The system can be easily customized by:
1. Updating the `councilData` object with new members
2. Modifying color schemes in CSS
3. Adjusting node sizes and layouts
4. Adding new sorting/filtering options
5. Extending data fields as needed

## 📈 Future Enhancements
Potential additions:
- Search functionality for members
- Filter by specific criteria
- Timeline view of council changes
- Vote tracking over time
- Connection strength visualization
- Export to various formats (PDF, PNG, SVG)
- Real-time data updates via API

## 👥 Council Members Included
1. Kerry P. Devine - Mayor
2. Charlie L. Frye, Jr. - Vice-Mayor (Ward 4)
3. Jannan W. Holmes - Council Member (At-Large)
4. Will B. Mackintosh - Council Member (At-Large)
5. Jason N. Graham - Council Member (Ward 1)
6. Jonathan A. Gerlach - Council Member (Ward 2)
7. Susanna R. Finn - Council Member (Ward 3)
8. Kelly J. Lackey - City Attorney
9. Timothy J. Baroody - City Manager
10. Josh Summits - Director, Economic Development & Tourism
11. Susan Spears - President & CEO, Chamber of Commerce

---

**Created**: 2025
**Version**: 2.0 (Tactical Interface Edition)
**License**: For research and educational purposes
