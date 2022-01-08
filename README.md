# macminix-040-cache-fix

Patch files for the [Mac Minix 040 cache fix](https://www.pliner.com/macminix/fix040.html),
retrieved from archive.org.

## Original Instructions

From: https://www.pliner.com/macminix/fix040.html

```
Thanks to Chris Hanson for this fix!

Here is what Chris posted to the comp.os.minix newsgroup:

Quite a while ago, I worked out how and when to flush caches so I could leave
my Centris' 040 running at full blast. This is the result of those efforts.
It adds an optional "flush040()" at two places, one in mm/exec.c and one in
mm/forkexit.c, and adds an assembly file to implement that routine to the memory
manager. On my Centris 610 I was getting 2000 dhrystones/sec with caches off on
a stock 1.5.10.7 kernel; with caches enabled and my new (not even optimized!)
kernel, I get around 7000. Happy, eh?

Share & enjoy,
Chris

PS - I'm guessing that this will work for 040 accelerators, and other M68000
machines using 040s. If anyone tries it, let me know, okay? :-)

Here are the directions he E-mailed me:
The file should end in .uue - it should be called something like 040sup.uue.
Notice under the "table" lines there's a line that says "begin XXX 040sup.tar.Z"
- this is the name of the output file to create once it's uudecoded; the
uuencoded file name should be 040sup.uue then.
macread "Disk:Path:patchfile.uue" | uud - > patchfile.tar.Z
zcat patchfile.tar | tar xvf -
Apply patches to files indicated in README, move files indicated in README to
appropriate spots.
```
