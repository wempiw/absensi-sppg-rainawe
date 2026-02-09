# TODO: Fix DoesNotExist Exception in Absensi Views

## Steps to Complete
- [x] Import necessary modules in absensi/views.py: `from django.contrib import messages` and `from django.core.exceptions import ObjectDoesNotExist`
- [x] Wrap `Pegawai.objects.get(user=request.user)` in try-except in `absen_masuk` function
- [x] Wrap `Pegawai.objects.get(user=request.user)` in try-except in `absen_pulang` function
- [x] Wrap `Pegawai.objects.get(user=request.user)` in try-except in `riwayat` function
- [x] Wrap `Pegawai.objects.get(user=request.user)` in try-except in `izin_list` function (in the else branch for non-admin)
- [x] Wrap `Pegawai.objects.get(user=request.user)` in try-except in `izin_create` function
- [x] Test the changes by running the Django server and accessing the /absensi/izin/ URL as a user without Pegawai profile
