* Benchmark CPU usage to try to figure out why we use ~100% while writing files.
* Implement "rarest-first" strategy where peers will prioritize files that they have that not many other peers do.
* Support torrents with multiple files.
* Support torrents with multiple trackers.
* Announce each X minutes to Tracker that you have a file.
* Announce to tracker when file completes.
* Instead of closing peer when Download completes, close it when neither peer is interested anymore?
* Only verify the file if it already existed on boot.
* Put file writing in a thread? (Measure time taken waiting for locks to see if this is delaying the PeerConnections.)
* Parallelize hash verification?
* Prioritize completing partially-completed pieces, to spread out hash calculation.
* With to_request changes, corrupted blocks won't get re-queued.
