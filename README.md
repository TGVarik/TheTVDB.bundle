## DEPRECATED 2017-02-13

As of Plex Media Server v1.4.1.3362-77c6a4f80, the TheTVDB.bundle that ships with PMS includes DVD-Order functionality. Please do not use this plugin anymore.

#### TheTVDB.bundle

Replace the bundle that comes with Plex with this one. 
On linux, that's: 

`/usr/lib/plexmediaserver/Resources/Plug-ins-xxxxxxx/TheTVDB.bundle` 

where `xxxxxxx` is the short-rev Plex appends to the end of their version strings. You need to check out the feature/dvd-order branch (git checkout feature/dvd-order); the default branch (latest; the one that gets checked out automatically when you git clone) is just the code for the most recently shipped version of the agent (the plexinc-agents/TheTVDB.bundle repository isn't up to date with production code). I update both branches automatically when installing a new version.

No need to switch agents for the shows that need DVD ordering. Go to 

`Settings -> Server -> Agents -> Shows -> TheTVDB` 

and click the gear next to the TheTVDB line to open the agent options. There's a new field to enter a comma-separated list of TVDB series ID numbers to use DVD ordering for. For example if you have Firefly, and S01E01 in your folder is "Serenity" and not "The Train Job", put 78874 in the field and then re-match the series ("fix incorrect match").

License
-------

If the software submitted to this repository accesses or calls any software provided by Plex (“Interfacing Software”), then as a condition for receiving services from Plex in response to such accesses or calls, you agree to grant and do hereby grant to Plex and its affiliates worldwide a worldwide, nonexclusive, and royalty-free right and license to use (including testing, hosting and linking to), copy, publicly perform, publicly display, reproduce in copies for distribution, and distribute the copies of any Interfacing Software made by you or with your assistance; provided, however, that you may notify Plex at legal@plex.tv if you do not wish for Plex to use, distribute, copy, publicly perform, publicly display, reproduce in copies for distribution, or distribute copies of an Interfacing Software that was created by you, and Plex will reasonable efforts to comply with such a request within a reasonable time.
