# Phala Incompatibilities (where SGX fuckin' suckz)

## Motherboards
The following motherboards have currently no compatibility with either SGX or Flexible Launch Control:
- Asus WS C246 DC (No full SGX compat)

## Processors
The following processors have limited/no compatibility with SGX
- Intel 7th Gen and below (No flexible launch control capabilities --> Level 5 confidence level)
- Any Intel Xeon aside from: E-2174G, E-2176G, E-2186G (Any other has limited compatibility, aim to get a processor with SGX with SPS support, not Intel ME)
