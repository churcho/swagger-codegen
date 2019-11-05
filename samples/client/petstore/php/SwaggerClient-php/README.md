# SwaggerClient-php
This spec is mainly for testing Petstore server and contains fake endpoints, models. Please do not use this for any other purpose. Special characters: \" \\

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Build package: io.swagger.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\AnotherFakeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\Client(); // \Swagger\Client\Model\Client | client model

try {
    $result = $apiInstance->testSpecialTags($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AnotherFakeApi->testSpecialTags: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *http://petstore.swagger.io:80/v2*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AnotherFakeApi* | [**testSpecialTags**](docs/Api/AnotherFakeApi.md#testspecialtags) | **PATCH** /another-fake/dummy | To test special tags
*DefaultApi* | [**testBodyWithQueryParams**](docs/Api/DefaultApi.md#testbodywithqueryparams) | **PUT** /fake/body-with-query-params | 
*FakeApi* | [**fakeOuterBooleanSerialize**](docs/Api/FakeApi.md#fakeouterbooleanserialize) | **POST** /fake/outer/boolean | 
*FakeApi* | [**fakeOuterCompositeSerialize**](docs/Api/FakeApi.md#fakeoutercompositeserialize) | **POST** /fake/outer/composite | 
*FakeApi* | [**fakeOuterNumberSerialize**](docs/Api/FakeApi.md#fakeouternumberserialize) | **POST** /fake/outer/number | 
*FakeApi* | [**fakeOuterStringSerialize**](docs/Api/FakeApi.md#fakeouterstringserialize) | **POST** /fake/outer/string | 
*FakeApi* | [**testClientModel**](docs/Api/FakeApi.md#testclientmodel) | **PATCH** /fake | To test \&quot;client\&quot; model
*FakeApi* | [**testEndpointParameters**](docs/Api/FakeApi.md#testendpointparameters) | **POST** /fake | Fake endpoint for testing various parameters 假端點 偽のエンドポイント 가짜 엔드 포인트
*FakeApi* | [**testEnumParameters**](docs/Api/FakeApi.md#testenumparameters) | **GET** /fake | To test enum parameters
*FakeApi* | [**testInlineAdditionalProperties**](docs/Api/FakeApi.md#testinlineadditionalproperties) | **POST** /fake/inline-additionalProperties | test inline additionalProperties
*FakeApi* | [**testJsonFormData**](docs/Api/FakeApi.md#testjsonformdata) | **GET** /fake/jsonFormData | test json serialization of form data
*FakeClassnameTags123Api* | [**testClassname**](docs/Api/FakeClassnameTags123Api.md#testclassname) | **PATCH** /fake_classname_test | To test class name in snake case
*PetApi* | [**addPet**](docs/Api/PetApi.md#addpet) | **POST** /pet | Add a new pet to the store
*PetApi* | [**deletePet**](docs/Api/PetApi.md#deletepet) | **DELETE** /pet/{petId} | Deletes a pet
*PetApi* | [**findPetsByStatus**](docs/Api/PetApi.md#findpetsbystatus) | **GET** /pet/findByStatus | Finds Pets by status
*PetApi* | [**findPetsByTags**](docs/Api/PetApi.md#findpetsbytags) | **GET** /pet/findByTags | Finds Pets by tags
*PetApi* | [**getPetById**](docs/Api/PetApi.md#getpetbyid) | **GET** /pet/{petId} | Find pet by ID
*PetApi* | [**updatePet**](docs/Api/PetApi.md#updatepet) | **PUT** /pet | Update an existing pet
*PetApi* | [**updatePetWithForm**](docs/Api/PetApi.md#updatepetwithform) | **POST** /pet/{petId} | Updates a pet in the store with form data
*PetApi* | [**uploadFile**](docs/Api/PetApi.md#uploadfile) | **POST** /pet/{petId}/uploadImage | uploads an image
*StoreApi* | [**deleteOrder**](docs/Api/StoreApi.md#deleteorder) | **DELETE** /store/order/{order_id} | Delete purchase order by ID
*StoreApi* | [**getInventory**](docs/Api/StoreApi.md#getinventory) | **GET** /store/inventory | Returns pet inventories by status
*StoreApi* | [**getOrderById**](docs/Api/StoreApi.md#getorderbyid) | **GET** /store/order/{order_id} | Find purchase order by ID
*StoreApi* | [**placeOrder**](docs/Api/StoreApi.md#placeorder) | **POST** /store/order | Place an order for a pet
*UserApi* | [**createUser**](docs/Api/UserApi.md#createuser) | **POST** /user | Create user
*UserApi* | [**createUsersWithArrayInput**](docs/Api/UserApi.md#createuserswitharrayinput) | **POST** /user/createWithArray | Creates list of users with given input array
*UserApi* | [**createUsersWithListInput**](docs/Api/UserApi.md#createuserswithlistinput) | **POST** /user/createWithList | Creates list of users with given input array
*UserApi* | [**deleteUser**](docs/Api/UserApi.md#deleteuser) | **DELETE** /user/{username} | Delete user
*UserApi* | [**getUserByName**](docs/Api/UserApi.md#getuserbyname) | **GET** /user/{username} | Get user by user name
*UserApi* | [**loginUser**](docs/Api/UserApi.md#loginuser) | **GET** /user/login | Logs user into the system
*UserApi* | [**logoutUser**](docs/Api/UserApi.md#logoutuser) | **GET** /user/logout | Logs out current logged in user session
*UserApi* | [**updateUser**](docs/Api/UserApi.md#updateuser) | **PUT** /user/{username} | Updated user


## Documentation For Models

 - [AdditionalPropertiesClass](docs/Model/AdditionalPropertiesClass.md)
 - [Animal](docs/Model/Animal.md)
 - [AnimalFarm](docs/Model/AnimalFarm.md)
 - [ApiResponse](docs/Model/ApiResponse.md)
 - [ArrayOfArrayOfNumberOnly](docs/Model/ArrayOfArrayOfNumberOnly.md)
 - [ArrayOfNumberOnly](docs/Model/ArrayOfNumberOnly.md)
 - [ArrayTest](docs/Model/ArrayTest.md)
 - [Capitalization](docs/Model/Capitalization.md)
 - [Category](docs/Model/Category.md)
 - [ClassModel](docs/Model/ClassModel.md)
 - [Client](docs/Model/Client.md)
 - [EnumArrays](docs/Model/EnumArrays.md)
 - [EnumClass](docs/Model/EnumClass.md)
 - [EnumTest](docs/Model/EnumTest.md)
 - [FormatTest](docs/Model/FormatTest.md)
 - [HasOnlyReadOnly](docs/Model/HasOnlyReadOnly.md)
 - [MapTest](docs/Model/MapTest.md)
 - [MixedPropertiesAndAdditionalPropertiesClass](docs/Model/MixedPropertiesAndAdditionalPropertiesClass.md)
 - [Model200Response](docs/Model/Model200Response.md)
 - [ModelList](docs/Model/ModelList.md)
 - [ModelReturn](docs/Model/ModelReturn.md)
 - [Name](docs/Model/Name.md)
 - [NumberOnly](docs/Model/NumberOnly.md)
 - [Order](docs/Model/Order.md)
 - [OuterBoolean](docs/Model/OuterBoolean.md)
 - [OuterComposite](docs/Model/OuterComposite.md)
 - [OuterEnum](docs/Model/OuterEnum.md)
 - [OuterNumber](docs/Model/OuterNumber.md)
 - [OuterString](docs/Model/OuterString.md)
 - [Pet](docs/Model/Pet.md)
 - [ReadOnlyFirst](docs/Model/ReadOnlyFirst.md)
 - [SpecialModelName](docs/Model/SpecialModelName.md)
 - [Tag](docs/Model/Tag.md)
 - [User](docs/Model/User.md)
 - [Cat](docs/Model/Cat.md)
 - [Dog](docs/Model/Dog.md)


## Documentation For Authorization


## api_key

- **Type**: API key
- **API key parameter name**: api_key
- **Location**: HTTP header

## api_key_query

- **Type**: API key
- **API key parameter name**: api_key_query
- **Location**: URL query string

## http_basic_test

- **Type**: HTTP basic authentication

## petstore_auth

- **Type**: OAuth
- **Flow**: implicit
- **Authorization URL**: http://petstore.swagger.io/api/oauth/dialog
- **Scopes**: 
 - **write:pets**: modify pets in your account
 - **read:pets**: read your pets


## Author

apiteam@swagger.io

