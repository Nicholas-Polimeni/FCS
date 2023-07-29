# QUESTIONS & DATA CONCERNS

## CMR
- There are many rows with the same Parid. Is this due to multiple buildings being on one parcel, with each building being recorded on a separate row? This did not appear to explain all the difference; usingg 'Bldnum' as a proxy for different buildings still yielded a small but not insignificant amount of left over duplicates.
- Why do some parcels seemingly have geocoded locations far outside Fulton county borders? This question applies to all datasets.
- What is the correct total number of commercial parcels in Fulton county?

## APPEALS
- No specific questions

## STANDARDS SALES
- What is a unique key to identify a transcation? Parid, Saledt is not unique, leaving 10% left over as duplicates. Why is this the case? Are these parcels with multiple buildings being sold?
- How is Fair Market Value calculated?
- Why are some saleprices recorded as 0?
- Taxyr is always one year ahead of sale year. Can you explain why?
- What explains the number of ParcelID duplicates? Grantor, Grantee, and assessor info alone does not seem to explain it. See some example cases in the notebook.

## STANDARDS DIGEST
- Why is there one file only labeled DIGEST 14th 2015...? The rest all follow the same pattern.
- NF + SF + ATL covers all parcels, correct? Does this include all types of parcels or is it only residential? E.g. do we need to combine CMR to this dataset to get the full universe?
- Any difference/reason between Own1 and Own2 columns?
- Why are some parcels from NF in SF and vice versa?

---

## MERGING CONERNS & GENERAL QUESTIONS
- Sometimes the spaces in the Parid are different in various datasets, even though they refer to the same parcel. Any harm in cleaning spaces? I know the online search feature doesn't work without the specific spaces.
- Grantee (sale data) vs owner (parcel data)- is there a delay in when the owner gets updated in the parcel data? E.g. if a property is sold in the later part a year, will the parcel data from that year still have the previous owner?
- Variable and parcel changes over the years? E.g. will variables be consistent over the years and do parcels change their IDs or get merged together or turned into separate parcels, etc.?
- Verify total number of parcels.
- Do you have geocoded data for all ParcelIDs?
- Any advice on matching parcel info to sales?