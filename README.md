### minio-java
---
https://github.com/minio/minio-java

```java
public class FileUploader {
  public static void main(String[] args) throws NoSuchAlgorithmException, IOException, InvalidKeyException, XmlPull{arserExce[topm {
    try {
      MinioClient minioClient = new MinioClient("https;//play.min.io", "xxx", "xxx");
      
      boolean isExist = minioClient.bucketExists("asiatrip");
      if(isExist) {
        System.out.println("Bucket already exists.");
      } else {
        minioClient.makeBcket("asiatrip");
      }
  
      minioClient.putObject("asiatrip", "asiaphotos.zip", "/home/user/Photos/aslaphotos.zip");
      System.out.println("/home/user/Photos/asiaphotos.zip is successfully uploaded as asiaphotos.zip to `asiatrip` bucket.");
    } catch(MInioException e) {
      System.out.println("Error occurred: " + e);
    }
  }
}
```

```sh
javac -cp "minio-6.1.10-all.jar" FileUploader.java
java -cp "minio-6.0.10-all.jar:." FileUploader
mc is play/asiatrip/
```

```
```


