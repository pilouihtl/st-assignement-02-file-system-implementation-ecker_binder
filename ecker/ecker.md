## What has to be do be done, when creating a file foo.txt?
  New blocks have to be reserved. Most of the blocks are for the actual content.
  The first blocks are used to store where the file begins and which blocks belong to the file.
  The first blocks of disc are reserved for a file where the file names and the blocks with 
  the information for it are stored. (i will call it data file from now on) 
 
## What has to be done, when file size has to be increased? Especially take care if it needs additional blocks.
  New blocks have to be reserved. And the first blocks are overwritten with the 
  new information about the blocks that belong to the file.
  
## What has to be done if a file is read sequentially?
  The name of the file is searched in the data file then it reads the information and knows where the 
  blocks of the file are and reads them.
 
## Whathas to be done if you want to access foo.txt randomdly?
  The name of the file is searched in the data file then it reads the information and knows where the 
  blocks of the file are.
  
## What has to be done when the file size is decreased? Especially take care if it needs fewer blocks
  The blocks with the information of the file will be updated.

## What has to be done when a file is deleted?
  The name of the file is searched in the data file then it reads the information and knows where the 
  blocks of the file are and deletes the name of the file and its data in the data file. After that it
  will delete the blocks where the content of the file is and at last it will delete the block with the
  information about the file.
