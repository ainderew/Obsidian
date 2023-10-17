look at index usage on the "index" tab


### Topics
- Wired Tiger Cache
- sparce index


sorting in memory: would be ok under 20k to sort in memory



![[Pasted image 20230905231136.png]]


ESR 
since b is an EQUALITY query and a is range query and c is a SORT query
![[Pasted image 20230905231224.png]]

![[Pasted image 20230905231549.png]]



FacilityAccountLink
need indexes 
 - facility._id
   
if the index doesn't start with the one your looking for it won't use the index
i.e 
**facData.masterFacId_facData.status.key_facData.facId_**
and if you look for **facData.facId** it wont use the index above since facData.facId isn't at the beginning.


POS Driver - load testing and randomized seeding