Intra42Api
=============

Intra42Api is an API wrapper.
Supports searches for Users, Campuses and Projects.

Installation
------------

**NOTE**: Python 3.9 or higher is required.

.. code:: python

   # Windows
   py -3.9 -m pip install intra42api

   # Linux
   python3.9 -m pip install intra42api

Example
-------

.. code:: python

	import intra42api

	intra = intra42api.Intra42()


	intra.setToken('MY_AWESOME_UID', 'MY_AWESOME_SECRET')


	user = intra.getUser('ID_OR_LOGIN')

	print(f"""
		Login: {user['login']}
		Email: {user['email']}
		Full Name: {user['displayname']}
		Correction Points: {user['correction_point']}
		url: {user['url']}
	""")