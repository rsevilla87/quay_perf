# Quay Perf Testing
## Assumptions
The Quay Operator has been deployed.

## Database
The database provided here is a dump from psql with a token generated for organization `test`

## Token
The default token is `opiqq6KJpCnn4YWqS4kkPku7pohjfzKX10EOGrUi`, after running the `quay_init.sh` script run the following

```
$ curl -k -X GET -H "Authorization: Bearer opiqq6KJpCnn4YWqS4kkPku7pohjfzKX10EOGrUi"  https://rook-quay-quay-openshift-quay.apps.rook43quay.perf-testing.devcluster.openshift.com/api/v1/superuser/users/
{"users": [{"username": "quay", "kind": "user", "verified": true, "name": "quay", "super_user": true, "enabled": true, "email": "changeme@example.com", "avatar": {"color": "#8c6d31", "kind": "user", "hash": "5cc105f67a24cab8379ad1cfd5dfdebb", "name": "quay"}}]}
```
