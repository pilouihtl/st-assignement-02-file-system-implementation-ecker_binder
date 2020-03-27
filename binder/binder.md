one block is split into the data component and another block with data component if one block is not enough for the file
at the end of the file is instead of another block a part with the system things like where is the start and where are the blocks in between located
then when a file is read sequentielly the blocks can easily read through
if the file is read randomly go to the extra block for the file at the end(not much time because the file data is at the bottom) and then go to the section of the file
when sth gets deleted the file data gets one block bottom ahead
