# Regera_nfce_python


Project to regenerate XMLs files for NFCe that is stored inside firebird database.
These files are compresed before write in database, this script:
Read from database, uncompress, transform XML to dictionary, apply changes, compress and save It to database.

There are 3 functions.

update_indPres  -> change tad indPres to 1.

update_csosn -> Change CSOSN to 500 when CFOP is 5405.

update_cfop -> Change cfop 5403 to 5405. According to NFCe project documentation, 5403 is not allowed to use.
