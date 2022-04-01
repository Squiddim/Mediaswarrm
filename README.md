---


---

<h1 id="mediaservarr">Mediaservarr</h1>
<p>In here you’ll find my Personal Configuration of various <a href="https://wiki.servarr.com/">*arr</a> &amp; other Homeserver Docker Containers. My Docker Swarm consists of multiple pies &amp; 1 x86 Host.</p>
<p>Note that some Container Tags are not device agnostic. Read the compose files carefully!</p>
<h2 id="containers-used">Containers used</h2>
<h3 id="frontends">Frontend('s)</h3>

<table>
<thead>
<tr>
<th>Container Name</th>
<th>Image</th>
<th>Referenced in</th>
<th>Use</th>
</tr>
</thead>
<tbody>
<tr>
<td>plex</td>
<td>linuxserver/plex:latest</td>
<td>content</td>
<td>Media Server</td>
</tr>
<tr>
<td>jellyfin</td>
<td>linuxserver/jellyfin:latest</td>
<td>content</td>
<td>FOSS Media Server</td>
</tr>
</tbody>
</table><h3 id="backend">Backend</h3>

<table>
<thead>
<tr>
<th>Container Name</th>
<th>Image</th>
<th>Referenced in</th>
<th>Use</th>
</tr>
</thead>
<tbody>
<tr>
<td>openvpn</td>
<td>dperson/openvpn-client:latest</td>
<td>content <br> !! own compose soon with traefik !!</td>
<td>VPN</td>
</tr>
<tr>
<td>deluge</td>
<td>linuxserver/deluge:latest</td>
<td>content</td>
<td>download client</td>
</tr>
<tr>
<td>jackett</td>
<td>linuxserver/jackett:latest</td>
<td>content</td>
<td>Proxy Server</td>
</tr>
<tr>
<td>sabnzbd</td>
<td>linuxserver/sabnzbd</td>
<td>content</td>
<td>Usenet Downloader</td>
</tr>
<tr>
<td>sonarr</td>
<td>linuxserver/sonarr:latest</td>
<td>content</td>
<td>RSS Indexer for Series</td>
</tr>
<tr>
<td>radarr</td>
<td>linuxserver/radarr:latest</td>
<td>content</td>
<td>RSS Indexer for Films</td>
</tr>
<tr>
<td>lidarr</td>
<td>linuxserver/lidarr:nightly</td>
<td>content</td>
<td>RSS Indexer for Music</td>
</tr>
<tr>
<td>readarr</td>
<td>linuxserver/readarr:nightly</td>
<td>content</td>
<td>RSS Indexer for Books</td>
</tr>
<tr>
<td>prowlarr</td>
<td>linuxserver/prowlarr:latest</td>
<td>content</td>
<td>Indexer Manager ( one place to add RSS Feeds )</td>
</tr>
<tr>
<td>bazaar</td>
<td>linuxserver/bazarr:latest</td>
<td>content</td>
<td>Manages Subtitles</td>
</tr>
</tbody>
</table><!---&#10;|  |  |  |  |&#10;|  |  |  |  |&#10;|  |  |  |  |&#10;|  |  |  |  |&#10;|  |  |  |  |&#10;|  |  |  |  |&#10;-->

