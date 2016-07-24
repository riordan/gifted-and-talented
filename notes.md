Notes
=======




# Networked File Structure:
Root structure:
 - `brightsign-dumps/` - empty directory
 - `feed_cache/` - empty directory
 - `pool/` - Asset storage. 2 directories deep. This is two levels deep, and the subdirectories are organized by the last two hex digits (oh fine, characters) of the sha1 hash of the file. SO... to make sense of this: a file with the sha1sum of `03cfd743661f07975fa2f1220c5194cbaff48451` would be located at `pool/5/1/sha1-03cfd743661f07975fa2f1220c5194cbaff48451`.
- `autoplugin.brs` - a do not delete warning
- `autorun.brs` - Presumibly a startup script
- `current-sync.xml` - manifest of what projects to download and run. This appears to be everything necessary for connection rules (where to go to download a future sync and credentials to do so), what projects to download (instructions on how to run a project - itself an xml file), media assets for a presentation, and the schedule which each presentation runs for