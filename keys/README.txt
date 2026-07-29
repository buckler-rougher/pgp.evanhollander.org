This folder is not committed as part of the site build — drop the real files
in here when the key is ready. The page fetches them client-side and shows
"not yet published" for anything missing, so it's safe to deploy before all
three files exist.

Email key (ProtonMail — Settings > Encryption and keys > Download public key):
  email-public.asc       the exported public key
  email-id.txt           short key ID, e.g. "3AA5C34371567BD2"
  email-fingerprint.txt  full fingerprint, spaced in groups of 4

Never put a .asc file containing a PRIVATE key in this folder — only ever
the public half. `gpg --armor --export` (not --export-secret-key) exports
the public key.
