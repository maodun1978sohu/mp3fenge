# directly cut out mp3 by time interval #
```
Mp3Fenge helper = new Mp3Fenge(new File("testdata/eyes_on_me.mp3"));
helper.generateNewMp3ByTime(new File("testdata/e1.mp3"), 307000, 315000);
```


# get mp3 data by time interval #
```
byte[] e2 = helper.getDataByTime(70000, 76000);
List<byte[]> mp3datas = new ArrayList<byte[]>();
mp3datas.add(e2);
FileUtil.generateFile(new File("testdata/e2.mp3"), mp3datas);
```