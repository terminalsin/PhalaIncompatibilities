# Phala Incompatibilities (where SGX fuckin' suckz)

## ✅ Recommendations 

### Motherboard / Racks
Any of the following motherboard have been known to mostly be compatible:

- X11SCM-F by SuperMicro [Link](https://www.supermicro.com/en/products/motherboard/X11SCM-F)
- X11SCW-F by SuperMicro [Link](https://www.supermicro.com/en/products/motherboard/X11SCW-F)
- R240 by Dell [Link](https://www.dell.com/fr-fr/work/shop/productdetailstxn/poweredge-r240)
- ProLient DL20 Gen10 by HP [Link](https://support.hpe.com/hpesc/public/docDisplay?docId=a00059854en_us&docLocale=en_US)
- RS100-E10-PI2 by Asus [Link](https://www.asus.com/fr/Commercial-Servers-Workstations/RS100-E10-PI2/)

### Processors
- Intel Xeon E-2276G
- Intel Xeon E-2278G
- Intel Xeon E-2286G
- Intel Xeon E-2288G
- Intel Xeon E-2176G
- Intel Xeon E-2178G
- Intel Xeon E-2186G
- Intel Xeon E-2188G
- Intel i9 9900K with corrected bios settings (updated firmware can fix most issues, albeit it will most the time be confidence level 4)

### BIOS Settings
- Disable Hypethreading
- Disable Speed-Shift
- Enable SGX
- Disable Secure-boot
- Disable Turbo-mode (if applicable)
- If you have a GPU, disable internal graphics. Do not disable if you do not have an integrated GPU.
- If applicable, switch to exclusively UEFI
- Ensure you're on the latest microcode update

## ⚠️ Known Incompatibilities 

### Motherboards
The following motherboards have currently no compatibility with either SGX or Flexible Launch Control:
- Asus WS C246 DC (No full SGX compat)

### Processors
The following processors have limited/no compatibility with SGX
- Intel 7th Gen and below (No flexible launch control capabilities --> Level 5 confidence level)
- Any Intel Xeon aside from: E-2174G, E-2176G, E-2186G (Any other has limited compatibility, aim to get a processor with SGX with SPS support, not Intel ME)
