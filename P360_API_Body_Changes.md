# API Body Changes

```diff
{
  "externalId": "25179",                          //🔵 Planlı Sipariş No
  "plannedSTartDate": "2026-01-14T14:30:00Z ",    //🔵 Planlanan Başlangıç Tarihi ve Saati
  "plannedSTartDate": "2026-01-14T15:30:00Z ",    //🔵 Planlanan Bitiş Tarihi ve Saati
  "materialCode": "1122334455",                   //🔵 Malzeme Kodu 
  "materialName": "12 DEMODENEME123 V1 EUROPE",   //🔵 Malzeme Tanımı
  "brand": "MARKA",                               //🔵 Marka
+ "modelGroup": "IC",                             //🔵 Chassiscode alanı
  "isWifi": "false",                              //🔵 ZFRT Malzemelerde (mamül) Zzkrpar WF ise true değilse false
- "barcode": "",                                  //🔴 DELETE
  "assetName": "MIX_BANT",                        //🔵 İşyeri 
  "serialNumbers": [                              //🔵 Barcode Listesi(Aybil DomesticCode)
   "1122334455261000710101",
   "1122334455261000700101",
   "1122334455261000690101",
   "1122334455261000680101",
   "1122334455261000670101",
   "1122334455261000660101",
   "1122334455261000650101",
   "1122334455261000640101",
   "1122334455261000630101",
   "1122334455261000620101",
   "1122334455261000610101",
   "1122334455261000600101",
   "1122334455261000590101",
   "1122334455261000580101",
   "1122334455261000570101"
  ],
  "quantity": 25,                               //🔵 Miktar 
  "description": "SAP üzerinden gelen iş emri", //🔵 Açıklama 
  "bom": {                                      //🔵 BOM Zzkrpar dolu olan malzemeler
    "description": "SAPBOMfor1122334455",       //🔵 Açıklama 
    "bomMaterials": [                           //🔵 Malzeme Listesi (HALB ROH ZHLB ZROH)   
      {
        "materialName": "1234567890",           //🔵 Malzeme Kodu 
        "quantity": 1,                          //🔵 Miktar 
        "isCritical": "FM",                     //🔵 Zzkrpar
-       "materialGroup": "MARKA",               //🔴 DELETE
+       "materialGroup": "Fan Motor",           //🔵 Marka yerine Krpartx
+       "MaterialUnitCode": "ST"                //🔵 Temel Ölçü Birimi
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "CP",
-       "materialGroup": "MARKA",
+       "materialGroup": "Compressor",
+       "MaterialUnitCode": "ST"
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "CB",
-       "materialGroup": "MARKA",
+       "materialGroup": "Control Box",
+       "MaterialUnitCode": "ST"
      },
      {
        "materialName": "1234567890",
        "quantity": 0.56,
        "isCritical": "R3",
-       "materialGroup": "MARKA",
+       "materialGroup": "R32 Refrigerant",
+       "MaterialUnitCode": "KG"
      },
      {
        "materialName": "1234567890",
        "quantity": 188,
        "isCritical": "R4",
-       "materialGroup": "R410A Refrigerant",
+       "MaterialUnitCode": "GR"
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "GG",
-       "materialGroup": "MARKA",
+       "materialGroup": "Guide Group",
+       "MaterialUnitCode": "ST"
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "GG",
-       "materialGroup": "MARKA",
+       "materialGroup": "Guide Group",
+       "MaterialUnitCode": "ST"
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "AC",
-       "materialGroup": "MARKA",
+       "materialGroup": "Accessories",
+       "MaterialUnitCode": "ST"
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "G",
-       "materialGroup": "MARKA",
+       "MaterialUnitCode": "ST"
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "HE",
-       "materialGroup": "MARKA",
+       "materialGroup": "Helium",
+       "MaterialUnitCode": "GR"
      },
      {
        "materialName": "1234567890",
        "quantity": 1,
        "isCritical": "GG",
-       "materialGroup": "MARKA",
+       "materialGroup": "Guide Group",
+       "MaterialUnitCode": "ST"
      }
    ]
  }
}
```
