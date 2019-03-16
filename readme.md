**My Edition Example**
```
AoBInput scanList = new AoBInput();
scanList.Add("LocalPlayer", "50 3F 9A FF");
scanList.Add("EntityList", "50 3F 9A AA");

AoBOutput result = await _memLib.AoBScan(StartAddress, EndAddress, scanList, true, true, "");
long LocalPlayerAddr = result["LocalPlayer"].FirstOrDefault();
List<long> EntityAddress = result["EntityList"];
```
----
