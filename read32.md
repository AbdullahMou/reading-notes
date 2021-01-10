
# Permissions

## permissions determining

* Permissions in REST framework are always defined as a list of permission classes.

## Object level permissions

* REST framework permissions also support object-level permissioning.
* Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

### Limitations of object level permissions

* For performance reasons the generic views will not automatically apply object level permissions to each instance in a queryset when returning a list of objects.

##  permission policy

* The default permission policy may be set globally, using the `DEFAULT_PERMISSION_CLASSES` setting

* You can also set the authentication policy on a per-view, or per-viewset basis, using the `APIView` class-based views.

## API Reference

### AllowAny
* The `AllowAny` permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.

* This permission is not strictly required, since you can achieve the same result by using an empty list or tuple for the permissions setting, but you may find it useful to specify this class because it makes the intention explicit.

### IsAuthenticated

* The `IsAuthenticated` permission class will deny permission to any unauthenticated user, and allow permission otherwise.

* This permission is suitable if you want your API to only be accessible to registered users.

### IsAuthenticatedOrReadOnly

* The `IsAuthenticatedOrReadOnly` will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

* This permission is suitable if you want to your API to allow read permissions to anonymous users, and only allow write permissions to authenticated users.

### Django Model Permissions

* This permission class ties into Django's standard django.contrib.auth model permissions. This permission must only be applied to views that have a .queryset property set. Authorization will only be granted if the user is authenticated and has the relevant model permissions assigned.

  * `POST` requests require the user to have the add permission on the model.
  * `PUT` and PATCH requests require the user to have the change permission on the model.
  * `DELETE` requests require the user to have the delete permission on the model. 

### Django Model Permissions Or AnonReadOnly

* Similar to `DjangoModelPermissions`, but also allows unauthenticated users to have read-only access to the API.

