# Layout
There are two styles of layout used in the project: full layout and blank layout.
___

## Full Layout
In FullLayout, there will be two main types of layout: vertical and horizontal layout, configured through redux - redux toolkit.


In src/store/customizer 
**State of layout**
![Layout State](/assets/images/layout-state.png)

**Actions of layout**
![Layout Action](/assets/images/layout-action.png)

### Navigation
![Navigations Structural](/assets/images/navigation-structural.png)

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| navlabel                     | boolean     | *undefined*    | Config true if title lable menu       |
| subheader                     | string     | *undefined*    | Title of menu       |
| subheaderI18n                     | string     | *undefined*    | Title via i18n of meny       |
| id                     | number     | *undefined*    | Key of menu       |
| title                     | string     | *undefined*    | Title of menu item      |
| titleI18n                     | string     | *undefined*    | Title via i18n of menu item      |
| icon                     | ReactNode     | *undefined*    | Icon prefix of menu      |
| href                     | string     | *undefined*    | Href of menu item      |
| isLayout                     | boolean     | *undefined*    | Toogle theme setting      |


### Impersonation

Check impersonation mode via redux - redux toolkit

```bash
  const isImpersonation = useSelector(getIsImpersonation);
```
If isImpersonation, change token to role impersonation and show alert inside header like that: 

```bash
    <Button
        aria-label="Impersonation"
        color="inherit"
        variant="text"
        aria-controls="msgs-menu"
        aria-haspopup="true"
        sx={{
         color: 'primary.main',
        }}
        onClick={() => dispatch(onImpersonationOut())}
        startIcon={<IconArrowBack size="15" style={{ marginTop: '2px' }} />}
    >
        {t('CORE:back_admin')}
    </Button>
```

```bash
  const accessToken = isImpersonation
    ? localStorage.getItem('impersonationToken')
    : localStorage.getItem('accessToken');
```

Assign the token to the base api method action like: 

```bash
    apiMethod.defaults.headers.common['Authorization'] = `Bearer ${accessToken}`;
```
### Testing Mode

Check testing mode via redux - redux toolkit
```bash
    const statusTesting = useSelector(getStatusTesting);
```
If statusTesting is `testing` show alert inside header, otherwise `null` allow create new test


## Blank Layout
Blank layout is used to show blank interface types without navigation bars such as: login registration, public user pages or warning pages.