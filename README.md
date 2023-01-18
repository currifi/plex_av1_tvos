<h1>Plex tvOS AV1 Client Profile</h1>

<h2>Issue:</h2><br />
When trying to play AV1 files using plex tvOS client, transcoding is initiated to h264.

<h2>Workaround:</h2><br />
Create <b>Profile</b> folder and copy the <b><a href="https://github.com/scriptsingh/plex_av1_tvos/blob/main/tvOS.xml">tvOS.xml</a></b> file to the folder and restart your Plex server. 

<h3>Example (ubuntu):</h3> 

Location of Plex data: <br />
/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/ <br />
<code>mkdir "/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/Profiles"</code> <br />
<code>nano "/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/Profiles/tvOS.xml"</code><br />
Copy contents from tvOS.xml to new file, save and reboot Plex server. <br />
Test Plex client on Apple TV. <br />

<b>For help finding Plex data location on other Operating Systems:</b><br /> 
https://support.plex.tv/articles/202915258-where-is-the-plex-media-server-data-directory-located/ 

Tested with smooth playback on latest Apple TV 4k and last gen model. 1st Gen model stutters on 1080p av1 and 4k content.
