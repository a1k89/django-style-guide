Django styleguide that I use in my projects.
### Testing

#### API

1. Create `tests` folder inside `api` module
2. Each api handler has own folder (for example, `auth`)
3. Naming: `test_<name_of_endpoint>`
4. Inside it, use naming: `<NameOfEndpoint>TestCase`

For example, your have `auth` api module with methods `auth_get_code`, `auth_enter_code`. 

`tests.auth.test_auth_enter_code`

```python
class AuthEnterCodeTestCase(BaseTestCase):
  pass
```

`tests.auth.test_auth_get_code`

```python
class AuthGetCodeTestCase(BaseTestCase):
  pass
```
