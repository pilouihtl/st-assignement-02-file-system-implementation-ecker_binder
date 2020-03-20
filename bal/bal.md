## What has to be done, when creating a file foo.txt?
A new block has to be reserved and then the WriteBlock() operation creates the file.

## What has to be done, when the file size has to be increased? Especially take care if it needs additional blocks
The first block has to be overwritten with WriteBlock().

## What has to be done if a file is read sequentially?
The ReadBlock() searches for the file name and then the data is read from the block.

## What has to be done if you want to access foo.txt randomdly(seek())?
The name gets searched in the block.

## What has to be done when the file size decreases? Especially take care if it needs fewer blocks
The block gets updated.

## What has to be done when a file is deleted?
The ReadBlock() operation searches for the file name and then once the flies are found, the name and data get deleted.
