# Accelerator Log

## Options
```json
{
  "apiDescription" : "",
  "apiOwner" : "",
  "apiSystem" : "",
  "artifactId" : "customer-profile",
  "buildTool" : "maven",
  "databaseMigrationTool" : "flyway",
  "databaseName" : "customer-profile-database",
  "exposeOpenAPIEndpoint" : false,
  "groupId" : "com.example",
  "javaVersion" : "11",
  "liveUpdateIDESupport" : true,
  "packageName" : "com.example.customerprofile",
  "projectName" : "customer-profile",
  "sourceRepositoryPrefix" : "dev.local"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(chain))
┃ ┃ ┃ engine.transformations[0].validated.chain (Let)
┃ ┃ ┃ Debug Adding symbol packageDirectory with value 'com/example/customerprofile'
┃ ┃ ┃ Debug Adding symbol workloadResourceName with value 'customer-profile'
┃ ┃ ┃ Debug Adding symbol databaseResourceName with value 'customer-profile-database'
┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Exclude, Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug build.gradle.kts matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.jar matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradle/wrapper/gradle-wrapper.properties matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug gradlew.bat matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug settings.gradle.kts matched [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [settings.gradle.kts, build.gradle.kts, gradlew*, gradle/**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug src/test/resources/application-test.properties didn't match [pom.xml, README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [<groupId>com.vmware.tap.accelerators</groupId>-><groupId>com.example...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/resources/application-test.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace regex '--- StartGradle[\s\S]+?--- EndGradle' with ''
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[1].sources[2].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '--- StartMaven\s|--- EndMaven\s' with ''
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[0].<combo>.transformations[2] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'gradle') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#databaseMigrationTool == 'flyway') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Exclude, Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃  Info Condition (#databaseMigrationTool == 'flyway') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [src/main/resources/db/changelog/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/db.changelog-master.xml matched [src/main/resources/db/changelog/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/changelog/V1.0__create_customer_profile_table.sql matched [src/main/resources/db/changelog/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [src/main/resources/db/changelog/**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, build.gradle.kts, **/application.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, build.gradle.kts, **/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [pom.xml, build.gradle.kts, **/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml didn't match [pom.xml, build.gradle.kts, **/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<dependency>\s+<groupId>org\.liquibase</groupId>\s+<artifactId>liquibase-core</artifactId>\s+</dependency>\s+' with ''
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[2].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [    implementation("org.liquibase:liquibase-core")->]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/application.properties]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**/application.properties] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/application.properties] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo>.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[1].sources[3].<combo>.transformations[2] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[2].<combo>.transformations[2] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[3] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#databaseMigrationTool == 'liquibase') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml matched [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml didn't match [config/postgres.yaml, config/workload-basic.yaml, config/workload-api-provider.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#exposeOpenAPIEndpoint) evaluated to false
┃ ┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (!#exposeOpenAPIEndpoint) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (!#exposeOpenAPIEndpoint) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload-basic.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml matched [config/workload-basic.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [config/workload-basic.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[2].<combo>.transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'config/workload-basic.yaml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yaml, folder=config/, filename=workload-basic.yaml, g0=config/workload-basic.yaml, g1=config/, g2=workload-basic.yaml, g3=workload-basic.yaml, g4=.yaml} and was rewritten to 'config/workload.yaml'
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-basic.yaml didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload-api-provider.yaml didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [config/workload.yaml, config/postgres.yaml, config/test-pipeline.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [rest-service-db->customer-profile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [customer-profile-database->customer-profile-dat...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[0].sources[3].<combo>.transformations[3] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [customerprofiledatabase->customer-profile-dat...(truncated)]
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[4].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseFirst))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(Merge(merge), UniquePath(UseLast)))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol workloadJavaVersion with value '11'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[0].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '<java.version>.*<' with '<java.version>11<'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex 'sourceCompatibility = .*' with 'sourceCompatibility ...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [build.gradle.kts]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [build.gradle.kts] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[2].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace regex '(?<unmodified>JavaVersion\.VERSION_)(\d+)' with '${unmodified}11'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[3].<combo>.transformations[1] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [config/*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [config/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug README.md didn't match [config/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [config/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [config/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [config/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug config/test-pipeline.yaml didn't match [config/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[0].sources[4].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace regex '(?<unmodified>image: bellsoft/liberica-openjdk-\w*:)(\d+)' with '${unmodified}11'
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[0].validated.merge.in.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[5].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'config/postgres.yaml', will use the one appearing first 
┃ ┃ ┃ ┃ ┃ ┃ Debug Multiple representations for path 'pom.xml', will use the one appearing first 
┃ ┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'config/test-pipeline.yaml', will use the one appearing first 
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseFirst))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Condition (#buildTool == 'maven') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [Tiltfile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug Tiltfile matched [Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [my-project->customer-profile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[0].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [dev.local->dev.local]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#liveUpdateIDESupport) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug Tiltfile didn't match [DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [my-project->customer-profile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[0].sources[1].<combo>.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [dev.local->dev.local]
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[0].validated.merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[6].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseFirst))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Combo, Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository != null) evaluated to false
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[0].validated.chain.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository == null) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug manifest.yaml matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ Debug README.md matched [**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug manifest.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[7].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Exclude
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[0].exclude (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**/*.java]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let(symbols, in: Chain(Include, chain...))
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1].<combo> (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol packageDirectory with value 'com/example/customerprofile'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1].<combo>.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1].<combo>.in.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.java]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java matched [**/*.java] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/*.java] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1].<combo>.in.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [com.vmware.tap.accelerators.restservicedb->com.example.customer...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[0].sources[1].<combo>.in.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/api/CustomerProfileControllerTest.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileControllerTest.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/api/CustomerProfileControllerTest.java} and was rewritten to 'src/test/java/com/example/customerprofile//api/CustomerProfileControllerTest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileServiceTest.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileServiceTest.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileServiceTest.java} and was rewritten to 'src/test/java/com/example/customerprofile//domain/CustomerProfileServiceTest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/ApplicationTests.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/ApplicationTests.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/ApplicationTests.java} and was rewritten to 'src/test/java/com/example/customerprofile//ApplicationTests.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileCreateRequest.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileCreateRequest.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileCreateRequest.java} and was rewritten to 'src/main/java/com/example/customerprofile//domain/CustomerProfileCreateRequest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileResponse.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileResponse.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileResponse.java} and was rewritten to 'src/main/java/com/example/customerprofile//domain/CustomerProfileResponse.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/api/CustomerProfileController.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/api/CustomerProfileController.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/api/CustomerProfileController.java} and was rewritten to 'src/main/java/com/example/customerprofile//api/CustomerProfileController.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=test, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/data/CustomerProfileRepositoryTest.java, g0=src/test/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepositoryTest.java, g1=test, g2=com/vmware/tap/accelerators/, g3=/data/CustomerProfileRepositoryTest.java} and was rewritten to 'src/test/java/com/example/customerprofile//data/CustomerProfileRepositoryTest.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/data/CustomerProfileEntity.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileEntity.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/data/CustomerProfileEntity.java} and was rewritten to 'src/main/java/com/example/customerprofile//data/CustomerProfileEntity.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/Application.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/Application.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/Application.java} and was rewritten to 'src/main/java/com/example/customerprofile//Application.java'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/domain/CustomerProfileService.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/domain/CustomerProfileService.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/domain/CustomerProfileService.java} and was rewritten to 'src/main/java/com/example/customerprofile//domain/CustomerProfileService.java'
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗ Debug Path 'src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java' matched 'src/(?<sourceset>.*)/java/(?<currentpackage>.*/)restservicedb(?<untouchedpath>.*)' with groups {sourceset=main, currentpackage=com/vmware/tap/accelerators/, untouchedpath=/data/CustomerProfileRepository.java, g0=src/main/java/com/vmware/tap/accelerators/restservicedb/data/CustomerProfileRepository.java, g1=main, g2=com/vmware/tap/accelerators/, g3=/data/CustomerProfileRepository.java} and was rewritten to 'src/main/java/com/example/customerprofile//data/CustomerProfileRepository.java'
┃ ┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[8].merge.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[9].merge (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[0].include (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/*.jar]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/*.jar] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Exclude, chain...)
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Exclude, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[1].<combo>.transformations[0] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [**/*.jar]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/db/migration/V1.0__create_customer_profile_table.sql didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/domain/CustomerProfileServiceTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/postgres.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/api/CustomerProfileController.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/api/CustomerProfileControllerTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/data/CustomerProfileRepositoryTest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/customerprofile/ApplicationTests.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileService.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/Application.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileResponse.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileEntity.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/domain/CustomerProfileCreateRequest.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/resources/application-test.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug docker-compose.yml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application-local.properties didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/customerprofile/data/CustomerProfileRepository.java didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug DEPLOYING.md didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug config/test-pipeline.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug manifest.yaml didn't match [**/*.jar] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[0].sources[1].<combo>.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [rest-service-db->customer-profile]
┃ ┗ ┗ ┗ ┗ ╺ engine.transformations[0].validated.chain.in.transformations[9].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
