# Mutt-Trash-Purge-patch
Updates of [Cedric Duval's 'trash' and 'purge' patches for mutt](http://cedricduval.free.fr/mutt/patches/)

These were originally two separate patches
- **trash** which moved deleted messages into a trash folder
- **purge** which actually deleted messages (depends on the trash patch)

I've merged them into a single patch (eliminating the dependency) and update them periodically so that they apply cleanly.
I haven't done extensive testing of these patches under 1.6.x, so use cautiously and let me know if something seems to break.

## How to apply these patches

1. Download the version of mutt you are interested in using from [mutt.org](http://www.mutt.org/)
2. Download the patch that matches the version of mutt you are using
3. Untar the source code for mutt
4. cd into the mutt folder
5. apply the patch

## Example

You can use the following commands to patch the latest version of mutt:

```
% wget ftp://ftp.mutt.org/pub/mutt/mutt-1.6.0.tar.gz
% wget https://raw.githubusercontent.com/kuperman/Mutt-Trash-Purge-patch/master/patch-1.6.0.bk.trash_folder-purge_message.1
% tar xzvf mutt-1.6.0.tar.gz
% cd mutt-1.6.0
% patch -p1 < ../patch-1.6.0.bk.trash_folder-purge_message.1
```
