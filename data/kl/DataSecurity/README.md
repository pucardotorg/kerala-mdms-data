# Data Security Policy

The data to be encrypted/decrypted is to be configured in terms of Attributes.

Attribute is defined as follows :
```
class Attribute {
    String jsonPath;
    String type;                //Used during encryption
    String maskingTechnique;    //Used during decryption
}
```

The enc/dec will be performed on JSON objects. The primary identifier of the Attribute is its jsonPath.

## Guidelines for Encryption Policy

```
class EncryptionPolicy {
    String key;
    List<Attribute> attrbutes;
}
```