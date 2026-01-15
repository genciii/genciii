# API Body Changes

```diff
{
  "externalId": "25179",                          //🔵 Planlı Sipariş No
  "plannedSTartDate": "2026-01-14T14:30:00Z ",    //🔵 Planlanan Başlangıç Tarihi ve Saati
  "plannedSTartDate": "2026-01-14T15:30:00Z ",    //🔵 Planlanan Bitiş Tarihi ve Saati
  "materialCode": "1122334455",                   //🔵 Malzeme Kodu 
  "materialName": "12 DEMODENEME123 V1 EUROPE",   //🔵 Malzeme Tanımı
  "brand": "MARKA",                               //🔵 Marka Karakteristikten Alacağız
+ "type": "RAC",                                  //🔵 Karakteristikten alacağız AL_ÜRÜN_ANA_GRUBU
+ "modelGroup": "IC",                             //🔵 Karakteristikten alacağız AL_İÇ_DIŞ (İç-Dış)
+ "chassisCode": "U4_4HP",                        //🔵 Karakteristikten alacağız AL_İÇ_ANA_ŞASİ/AL_DIŞ_ANA_ŞASİ (İç-Dış-U4_4HP)
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
-   "description": "SAPBOMfor1122334455",       //🔴 DELETE
    "bomMaterials": [                           //🔵 Malzeme Listesi (HALB ROH ZHLB ZROH)   
      {
-       "materialName": "1234567890",           //🔴 DELETE
+       "materialCode": "1234567890",           //🔵 Malzeme Kodu
+       "materialName": "Malzeme",              //🔵 Malzeme Tanımı
        "quantity": 1,                          //🔵 Miktar 
        "isCritical": "FM",                     //🔵 Zzkrpar
-       "materialGroup": "MARKA",               //🔴 DELETE
+       "criticalDescription": "Fan Motor",     //🔵 Marka yerine Krpartx
+       "materialUnitCode": "ST"                //🔵 Temel Ölçü Birimi
      },
      {
-       "materialName": "1234567890",          
+       "materialCode": "1234567890",          
+       "materialName": "Malzeme",              
        "quantity": 1,
        "isCritical": "CP",
-       "materialGroup": "MARKA",
+       "criticalDescription": "Compressor",
+       "materialUnitCode": "ST"
      },
      {
-       "materialName": "1234567890",           
+       "materialCode": "1234567890",           
+       "materialName": "Malzeme",              
        "quantity": 1,
        "isCritical": "CB",
-       "materialGroup": "MARKA",
+       "criticalDescription": "Control Box",
+       "materialUnitCode": "ST"
      },
      {
-       "materialName": "1234567890",          
+       "materialCode": "1234567890",           
+       "materialName": "Malzeme",              
        "quantity": 0.56,
        "isCritical": "R3",
-       "materialGroup": "MARKA",
+       "criticalDescription": "R32 Refrigerant",
+       "materialUnitCode": "KG"
      },
      {
-       "materialName": "1234567890",           
+       "materialCode": "1234567890",           
+       "materialName": "Malzeme",             
        "quantity": 188,
        "isCritical": "R4",
-       "criticalDescription": "R410A Refrigerant",
+       "materialUnitCode": "GR"
      },
      {
-       "materialName": "1234567890",           
+       "materialCode": "1234567890",           
+       "materialName": "Malzeme",             
        "quantity": 1,
        "isCritical": "GG",
-       "materialGroup": "MARKA",
+       "criticalDescription": "Guide Group",
+       "materialUnitCode": "ST"
      },
      {
-       "materialName": "1234567890",          
+       "materialCode": "1234567890",           
+       "materialName": "Malzeme",             
        "quantity": 1,
        "isCritical": "GG",
-       "materialGroup": "MARKA",
+       "criticalDescription": "Guide Group",
+       "materialUnitCode": "ST"
      },
      {
-       "materialName": "1234567890",          
+       "materialCode": "1234567890",           
+       "materialName": "Malzeme",            
        "quantity": 1,
        "isCritical": "AC",
-       "materialGroup": "MARKA",
+       "criticalDescription": "Accessories",
+       "materialUnitCode": "ST"
      },
      {
-       "materialName": "1234567890",          
+       "materialCode": "1234567890",          
+       "materialName": "Malzeme",           
        "quantity": 1,
        "isCritical": "G",
-       "criticalDescription": "MARKA",
+       "materialUnitCode": "ST"
      },
      {
-       "materialName": "1234567890",       
+       "materialCode": "1234567890",         
+       "materialName": "Malzeme",             
        "quantity": 1,
        "isCritical": "HE",
-       "materialGroup": "MARKA",
+       "criticalDescription": "Helium",
+       "materialUnitCode": "GR"
      },
      {
-       "materialName": "1234567890",         
+       "materialCode": "1234567890",           
+       "materialName": "Malzeme",            
        "quantity": 1,
        "isCritical": "GG",
-       "materialGroup": "MARKA",
+       "criticalDescription": "Guide Group",
+       "materialUnitCode": "ST"
      }
    ]
  }
}
```
