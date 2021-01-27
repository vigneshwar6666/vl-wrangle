# vl-wrangle

## Fetching with Bash.
curl "http://shakespeare.mit.edu/richardii/full.html" | sed 's/<\/*[^>]*>//g' > R2.txt

## To find matches with Bash
1. grep -i 'KING RICHARD II' Richard2.txt -c
2. cat Richard2.txt | grep -i 'KING RICHARD II' -c
3. at R2.txt | grep -i 'KING RICHARD II'
4. grep -iv 'KING RICHARD II' R2.txt
5. grep -i 'HENRY BOLINGBROKE' R2.txt
6. grep -i 'HENRY BOLINGBROKE' R2.txt -c
7. tr ' ' '\12' < R2.txt | sort | uniq -c | sort -nr > result.txt

## To preview content with Bash (cat, head, tail)
1. cat result.txt
2. head -10 result.txt
3. tail -4 result.txt
