$watcher = New-Object System.IO.FileSystemWatcher
$watcher.Path = get-location
$watcher.IncludeSubdirectories = $true
$watcher.EnableRaisingEvents = $false
# Changes filter, last time written and filename
$watcher.NotifyFilter = [System.IO.NotifyFilters]::LastWrite -bor [System.IO.NotifyFilters]::FileName

while($TRUE){
	$result = $watcher.WaitForChanged([System.IO.WatcherChangeTypes]::Changed -bor [System.IO.WatcherChangeTypes]::Renamed -bOr [System.IO.WatcherChangeTypes]::Created, 1000);
	if($result.TimedOut){
		# Skip this iteration only and return back to the top of the loop. Timedout without changes.
		continue;
	}
	# Avoid locked file once being copied
	sleep 1;
	write-host -foreground yellow "Change in " + $result.Name
	.\ConsoleAppAD.exe
}
