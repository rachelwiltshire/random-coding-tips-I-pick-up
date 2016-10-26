# random-coding-tips-I-pick-up
Finally, somewhere sensible to keep these rather than the post-its on my monitors!

## Linux

### To view binary files
xxd -b file.bed

### To create a symbolic link
ln -s /path-to-shortcut

### To move the cursor in the line
control + a (beginning)
control + e (end)

## R

### To remove rows and columns from a matrix
I hit this problem frequently when attempting to make my geographical and Fst matrices even for Isolation By Distance regression
data <- data[-(R:R),-(C:C)] or [-R:-R,-C:-C]
