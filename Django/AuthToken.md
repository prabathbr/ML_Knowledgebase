# Django Auth Token

###References:
- DRF source code (Token Model) = https://github.com/encode/django-rest-framework/blob/master/rest_framework/authtoken/models.py
- Algorithm = https://stackoverflow.com/questions/14567586/token-authentication-for-restful-api-should-the-token-be-periodically-changed
- Algorithm = https://chrisbartos.com/articles/how-to-override-tokenauthentication-backend-to-detect-an-expiring-token/
- Algorithm = https://medium.com/@yerkebulan199/django-rest-framework-drf-token-authentication-with-expires-in-a05c1d2b7e05

### Extend Auth Token Expiry

Extend the active token's validity time by another given time (ex:15min) just by setting the current token's creation time to current time,

Based on  : https://medium.com/@yerkebulan199/django-rest-framework-drf-token-authentication-with-expires-in-a05c1d2b7e05
	
	def token_expire_handler(token):
	    is_expired = is_token_expired(token)
	    if is_expired:
	        token.delete()
	        token = Token.objects.create(user = token.user)
	    elif not is_expired: # time reset
	        token.created = timezone.now() # time reset
	        token.save() # time reset
	    return is_expired, token