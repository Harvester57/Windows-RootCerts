﻿# Windows-RootCerts

Latest certs can be downloaded through Windows Update, on a computer with internet access, with the following command:
       certutil.exe -syncWithWU -f $Path

This will download all Root Certs unitarily. This will also download the authrootstl.cab and disallowedcertstl.cab files, that we need to expand to get the corresponding .stl files.

We also add the Root Certs and CRLs obtained through WSUS Offline, just in case of (but that might be redundant with the certs downloaded through certutil.exe).
