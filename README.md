Transparent Data Encryption (TDE)

1.Create a master key in the master database.
2.Create a certificate in the master database.
3.Backup the certificate and private key securely.
4.Switch to the target database you want to encrypt.
5.Create a database encryption key in the target database.
6.Enable encryption on the database using the encryption key.
7.Verify encryption status using sys.dm_database_encryption_keys.
8.Wait until encryption_state becomes 3 (encrypted).
9.Ensure certificate backups are stored safely for restore.


✅ SQL Server Encryption States (7 States)

0 – No encryption

1 – Unencrypted

2 – Encryption in progress

3 – Encrypted

4 – Key change in progress

5 – Decryption in progress

6 – Protection change in progress
