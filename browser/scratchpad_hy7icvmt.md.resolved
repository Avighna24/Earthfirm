# Earthfirm Sports Infra Cost Estimator Verification

## Checklist
- [x] Navigate to the Project Cost Estimator section
- [x] Observe active item selection for Step 1 (Basketball should highlight)
- [x] Click 'Football Turf' and verify its border highlights (taking brandGreen border class)
- [x] Click 'Next Step' to go to Step 2
- [x] Verify 'Standard Size' and 'Existing Concrete Base' start highlighted
- [x] Click 'Premium / Large Size' and see if its border highlights while 'Standard Size' loses its border highlight
- [x] Click 'Full Excavation & Civil Work' and see if its border highlights
- [x] Click 'Next Step' to go to Step 3
- [x] Click 'LED Flood Lighting System' and verify it highlights
- [x] Report if all selections correctly shifted the brandGreen border style to the active options

## Findings
1. **Step 1 (Sports selection):** Transition works perfectly. Clicking 'Football Turf' successfully highlights its border with the `border-brandGreen` class, while 'Basketball Court' correctly loses its green border (though the `active` text class remains on 'Basketball Court', the visual border updates correctly).
2. **Step 2 (Size Category & Sub-Base):**
   - Both 'Standard Size' and 'Existing Concrete / Asphalt Base' start with active green border styling (`border-brandGreen bg-slate-900/60`) hardcoded on their parent `<label>` elements.
   - When clicking 'Premium / Large Size' or 'Full Excavation & Civil Work', the checkbox/radio inner circles correctly update/fill with green (native browser behavior), but **their parent `<label>` border classes do not shift**. The green borders remain hardcoded on 'Standard Size' and 'Existing Concrete / Asphalt Base'.
3. **Step 3 (Optional Upgrades):**
   - Both checkboxes start with default white borders (`border-white/10 bg-slate-900/40`).
   - When selecting 'LED Flood Lighting System', the checkbox correctly fills with green, but **the parent `<label>` border class does not shift** to the brandGreen border style.

## Conclusion
Selections do not correctly shift the `brandGreen` border style to the active options in Step 2 and Step 3. The green border highlights are hardcoded on the default-selected options of Step 2, and are missing entirely from Step 3 options, even when active. Only Step 1 correctly updates the border styling dynamically when a sport card is clicked.

