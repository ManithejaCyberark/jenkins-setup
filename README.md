# public-keys update #
## Requirement
+ Jenkins Server
+ Conjur Secrets plugin
+ Conjur Server
+ Conjur Policies
  * the host or user should have permission to only update the public-keys.
  * Here an Example
    ```
    - !permit
      resource: !variable conjur/authn-jwt/jenkins/public-keys
      privileges: [ update ]
      roles: !host jenkins/projects/jenkins
    ```

## Usage instructions
### Step by step guide
![image](https://github.com/ManithejaCyberark/public-keys-update/assets/109070761/1549416a-83c7-440f-8565-f95b3ccc1e6a)
