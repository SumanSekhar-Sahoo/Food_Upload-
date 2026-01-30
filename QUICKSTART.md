# Quick Start Guide

## 🚀 View the Page

### Option 1: Direct Browser Open
1. Navigate to: `d:\Desktop\Web clg\FoodUpload\index.html`
2. Right-click → Open with → Your browser
3. Or drag the file into your browser window

### Option 2: Using VS Code Live Server
1. Install "Live Server" extension (if not already installed)
2. Right-click on `index.html`
3. Select "Open with Live Server"
4. Page opens in `http://localhost:5500/index.html`

### Option 3: Python Simple Server
```bash
cd "d:\Desktop\Web clg\FoodUpload"
python -m http.server 8000
```
Then open: `http://localhost:8000`

---

## ✨ What You'll See

### The Complete Form
A clean, professional full-screen page with:
- **Large centered heading** at the top
- **Form sections** flowing naturally down the page
- **Large drag-and-drop upload area** for images
- **Price toggle** to switch between Free/Paid
- **Two action buttons** at the bottom center

### Test These Features

#### 1. Upload Image
- Hover over the upload area → see hover effect
- Click to browse or drag an image onto the area
- Image preview appears below the upload area
- Click ✕ button to remove image

#### 2. Price Toggle
- Look for "Price Information" section at the bottom
- **Click the toggle switch**:
  - OFF (blue) = "Free Food" → Price shows ₹0 (disabled)
  - ON (green) = "Paid Food" → Price input becomes editable
- Try typing a price when enabled

#### 3. Expiry Date
- Select a future date in the Expiry Date field
- See the countdown: "Expires in X days"

#### 4. Form Submission
- Try clicking "Add Food Item" without filling required fields
- Red error messages appear under empty required fields
- Fill all required fields → green success message appears
- Form automatically resets

#### 5. Responsive Design
- **Resize your browser** to see mobile layout
- At 640px width and below:
  - Form fields stack in single column
  - Buttons stack vertically
  - Font sizes adjust for readability

---

## 🎨 Design Details

### Color Palette
| Element | Color | Usage |
|---------|-------|-------|
| Primary | #5F6F52 | Buttons, active states, headings |
| Background | #FAFAF8 | Page background (soft off-white) |
| Text Primary | #1F2933 | Main text, labels |
| Text Secondary | #6B7280 | Help text, descriptions |
| Border | #E5E7EB | Form input borders |
| Error | #DC2626 | Error messages |
| Success | #10B981 | Success messages |

### Typography Sizes
- **Page Title**: 44px (bold)
- **Subtitle**: 17px (regular)
- **Section Titles**: 13px (uppercase, bold)
- **Form Labels**: 15px (semi-bold)
- **Form Inputs**: 15px
- **Button Text**: 16px (semi-bold)

### Spacing
- **Section gaps**: 48px
- **Column gaps**: 28px
- **Component padding**: 12-16px internal

---

## 📋 Form Fields Included

### Required Fields (marked with *)
- Food Name
- Category
- Food Image
- Quantity
- Expiry Date

### Optional Fields
- Food Description
- Storage Type
- Food Condition
- Pickup Availability
- Location
- Notes
- Price (only required if "Paid Food" is selected)

---

## 🔧 Customization Tips

### Change the Color Scheme
In `index.html`, find the `:root` section (~line 16):
```css
:root {
    --primary: #5F6F52;  /* Change this color */
    --background: #FAFAF8;
    --text-primary: #1F2933;
    /* ... more colors ... */
}
```

### Adjust Form Padding
Find `.main-content` (line ~87):
```css
.main-content {
    padding: 60px 24px 100px 24px;  /* top, sides, bottom */
}
```

### Modify Button Text
In the HTML form section, update button labels:
```html
<button type="submit" class="btn-primary">Add Food Item</button>
<button type="reset" class="btn-secondary">Clear Form</button>
```

---

## 💡 Key Features

✅ **Full-screen, no sidebar** - Clean, focused workflow  
✅ **Responsive design** - Works on mobile, tablet, desktop  
✅ **Price toggle** - Switch between free and paid options  
✅ **Image preview** - See uploaded images before submission  
✅ **Form validation** - Required fields must be filled  
✅ **Expiry countdown** - Automatic day calculation  
✅ **Accessibility** - Keyboard navigation, ARIA labels  
✅ **Professional UI** - Dashboard-grade styling  

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| Page looks blank | Check browser console (F12) for JS errors |
| Upload area not working | Ensure JavaScript is enabled |
| Toggle not working | Check that IDs match in HTML and CSS |
| Buttons not centered | Check CSS media queries for your screen size |
| Colors look wrong | Clear browser cache (Ctrl+Shift+Delete) |

---

## 📞 Support

For questions or issues:
1. Check the `CHANGES.md` file for detailed documentation
2. Review the CSS variables in `index.html` for styling
3. Check browser console (F12 → Console tab) for errors
4. Verify all form field IDs match between HTML and JavaScript

Enjoy your new FoodShare form! 🎉
