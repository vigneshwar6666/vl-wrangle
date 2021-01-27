# vl-wrangle
## Fetching with Bash.
curl "http://shakespeare.mit.edu/richardii/full.html" | sed 's/<\/*[^>]*>//g' > R2.txt
## To find matches with Bash
grep -i 'KING RICHARD II' Richard2.txt -c
cat Richard2.txt | grep -i 'KING RICHARD II' -c
cat R2.txt | grep -i 'KING RICHARD II'
grep -iv 'KING RICHARD II' R2.txt
grep -i 'HENRY BOLINGBROKE' R2.txt
grep -i 'HENRY BOLINGBROKE' R2.txt -c
tr ' ' '\12' < R2.txt | sort | uniq -c | sort -nr > result.txt
## To preview content with Bash (cat, head, tail)
cat result.txt
head -10 result.txt
tail -4 result.txt
