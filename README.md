# pi-topOS Network Modifications

This package currently manages a udev rule that ensures that wireless devices do not enter power save mode.

It also turns on NetworkManager's connectivity check (Debian's `network-manager-config-connectivity-debian`). Without it NetworkManager reports full connectivity on any network that gives an address, so a pi-top behind a Wi-Fi sign-in page (captive portal) can't tell. With it, NetworkManager reports `portal`, and pt-miniscreen shows how to sign in.
