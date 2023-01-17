Plex tvOS AV1 Client Profile

Issue:
When trying to play AV1 files using plex tvOS client, transcoding is initiated to h264.

Workaround:
Create Profile folder and copy the tvOS.xml file to the folder and restart your plex server and test. 
Example (ubuntu): 
Location of Plex data: 
/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/
mkdir "/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/Profiles"
nano "/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/Profiles/tvOS.xml"
Copy contents from tvOS.xml to new file, save and reboot plex.
Test plex client on Apple TV. 
For help finding Plex data location: https://support.plex.tv/articles/202915258-where-is-the-plex-media-server-data-directory-located/ 
