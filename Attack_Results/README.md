Attack results evidence files.
The attack results were analyzed using traffic generation proof, Wireshark packet analysis, and final forensic correlation through Zeek and Loki dashboards.

The traffic generation proof confirmed that the attacker successfully created a connection between Computer A and Computer B using Java FileSender through port 5001. The file important.docx was transferred successfully, proving unauthorized file movement inside the network.

The Wireshark attack timeline chart showed active TCP communication between 192.168.17.137 and 192.168.17.134 through port 5001. The packet flow and increasing byte transmission helped identify the exact attack start time, transfer period, and suspicious connection behavior.

The final analysis result from Loki and Zeek confirmed active connection reuse, exact timestamps, and suspicious file transfer activity between both systems. The logs verified the communication path and supported the final forensic investigation.

By combining these results with Grafana monitoring and Prometheus system tracking, the security team successfully identified the attacker, confirmed the stolen file, determined how the transfer happened, and completed the full DDoS and file transfer investigation with strong multi source forensic evidence.
