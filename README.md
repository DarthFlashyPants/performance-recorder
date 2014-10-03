Sithy Performance Recorder
=========

An unsupported alternate performance recorder report which adds some extra stuff

Windows:

 
```sh
 -Navigate to C:\Program Files\Tableau\Tableau 8.2\Performance
 -Rename PerformanceRecording_new.twb to PerformanceRecording_new.old
 -Drop the Sithy version in. 
```


Mac:

```sh
 - In Applicatons folder, right-click Tableau and select "Show Package Contents"
 - Navigate to /Contents/install/Performance
 - Rename PerformanceRecording_new.twb to PerformanceRecording_new.old
 - Drop the Sithy version in.
```

Notes
----
For reasons unknown to this Sith, it seems that if one stops the performance recorder immediately after a viz has rendered, then the "Cache Hit" field often comes back Null ("Not Applicable") across the board. When this occurs, query text is also empty. Perhaps this is why the field wasn't used by Tableau out of the box?

Try waiting at least few seconds after your sheet renders before stopping the recorder and your results should come back more dependably.