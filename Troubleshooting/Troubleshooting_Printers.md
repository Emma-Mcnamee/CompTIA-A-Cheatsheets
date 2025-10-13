# Troubleshooting Printers

## Testing the Printer
- Print or scan a test page (built into Windows).  
- Use diagnostic tools such as web-based utilities or manufacturer software.  

## Bad Output
- **Lines down the page:** Clean print heads or check for a scratched photosensitive drum.  
- **Faded print:** Low toner or ink.  
- **Double images:** Optical drum not cleaning properly.  

### Garbled Print
- Incorrect or corrupted printer driver (wrong model configured in Windows).  
- Incorrect page description language (PCL vs PostScript).  
- Verify printer functionality with a test page.  
- Test the same job in a different application—if it prints fine, upgrade or repair the app.  

## Paper Jam
- Remove carefully to avoid tearing paper and leaving scraps inside.  
- Check the tray and **pickup rollers**—these wear out and are replaced via a maintenance kit.  
- **Creased paper:** Caused by problems in the paper path or wrong paper weight.  

## Multiple Prints Pending in Queue
- Printer spooler may crash or freeze—most systems auto-restart it.  
- Check **Event Viewer** for logged issues.  
- A single corrupted print job can block the entire queue.  

## Grinding Noise
- Indicates mechanical failure: paper jam, carriage jam, or stalled mechanism.  
- Refer to the printer’s manual for specific troubleshooting steps.  
- Could indicate a failing internal part—may require service or replacement.  

## Finishing Issues
- Occur after the ink or toner has been applied.  
- **Staple jams:** Large multifunction printers collate and staple sets of paper; check the manual for clearing procedures.  
- **Hole punches misaligned:** Verify alignment settings in the printer driver.  

## Incorrect Page Orientation
- Check driver settings (portrait/landscape) before printing.  
- May require a driver update.  
- Some printers also have physical orientation settings in their onboard menus.  

## Tray Not Recognized
- Printers often have multiple trays with different paper sizes or types.  
- Ensure paper size in the driver matches the tray’s physical configuration.  
- Tray definitions are set in the **driver configuration**.  

## Connectivity Issues
- Verify the printer is on the network and properly connected.  
- Confirm IP address, subnet mask, default gateway, and DNS settings.  
- If network-based, check printer server connection and configuration.  
