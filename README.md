# Torrent Tracker IPs Blacklist

This repository contains a list of known torrent tracker IPs in the file `extracted_ips.txt`. The list can be used for any purpose, including blocking public torrent trackers to reduce the risk of being flagged by copyright owners while torrenting.

## Contents

- `extracted_ips.txt`: A plain text file containing a list of IP addresses of known torrent trackers.

## Purpose

This list was originally curated to blacklist public torrent trackers, minimizing the chances of IP detection by copyright monitoring entities. However, you are free to use this list for any other purpose as per your requirements.

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/torrent-tracker-ips-blacklist.git
   cd torrent-tracker-ips-blacklist
   ```

2. Use the extracted_ips.txt file in your network configuration or blocking rules.

Example: Blocking IPs using iptables (Linux):

```bash
while read -r ip; do
    sudo iptables -A INPUT -s $ip -j DROP
done < extracted_ips.txt
```

3. Integrate into scripts or applications as needed.

## Disclaimer

No Guarantees: This list may not be exhaustive or completely up-to-date. Some IPs may no longer be associated with torrent trackers, while new ones may exist.
Use at Your Own Risk: The author is not responsible for any issues caused by the use of this list, including but not limited to accidental blocking of legitimate services.
Contributing
If you find additional torrent tracker IPs or notice inaccuracies in the list, feel free to contribute:

## Fork this repository.

Update extracted_ips.txt with the new or corrected IPs.
Create a pull request with a detailed explanation of your changes.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
