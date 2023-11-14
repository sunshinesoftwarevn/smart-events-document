# Components directory

The components directory contains your React.Js Components. Components are what makes up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

___

## Admin Tables
---
This component is a defined table with fetching data via static structural common for all systems.

![Admin Table Structural](/assets/images/admin-table-structural.png)

The structural structure of these components contains the core table, dynamic filter action, and styles.
To get started, please continue with the **index.js** file.

**Component API:**

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| api                     | `Functional`      | *undefined*    | Api gets a list to show        |
| defs                    | object          | *undefined*    | Config table of columns via [table antd](https://4x.ant.design/components/table/#Column)        |
| showCheckbox            | boolean         | true           | Config to show or hide a checkbox        |
| showDeleteItem          | boolean         | true           | Config to show or hide a delete action        |
| showPagination          | boolean         | false          | Config to show or hide a pagination        |
| defaultPageSize         | number          | 20             | Limit of list        |
| rowKey                  | string          | "id"           | Key of row        |
| apiDelete               | `Functional`      | *undefined*    | Api functional for delete action        |
| afterDeleteSuccess      | `Functional`      | *undefined*    | Action after delete success        |
| loading                 | boolean         | false          | Loading table        |
| treeMode                | boolean         | false          | Tree mode        |
| scroll                  | object          | Default scroll | Config scroll        |
| modeRowKeys             | object          | *undefined*    |         |
| disableAllCheckbox      | boolean         | false          | Disabled all checkbox        |
| disableCheckboxKey      | boolean         | false          | Disabled all checkbox key        |
| disableCheckboxFunction | boolean         | false          | Disabled all checkbox function        |
| rowKeysChange           | `Functional`      | false          | Handle change keys action        |
| scrollToFirstRowOnChange| boolean         | true           | Scroll to first when row changed        |
| conditionShowDeleteItem | `Functional`      | *undefined*    | Conditional to show delete        |
| customRequestDelete     | object          | *undefined*    | Custom request delete action        |
| bordered                | boolean         | true           | Border of table        |
| customAction            | `Functional`      | *undefined*    | Custom Action of Action columns        |
| showEditItem            | boolean         | false          | Show edit item        |
| editPathRoute           | `Functional`      | *undefined*    | Route or action to edit item       |
| typeAction              | string          | *undefined*    | Type action of action columns         |
| menuAction              | Functional      | *undefined*    | Menu item of action columns        |
| renderAction            | Functional      | *undefined*    |         |
| onGroupRowAction        | Functional      | *undefined*    |         |
| fixedValuesFilter       | object          | *undefined*    | Values filter fixed        |
| searchPlaceHolder       | string          | 'CORE:search_holder'    | Placeholder of search        |
| customRightAction       | `Functional`          | *undefined*    | Right action        |
| customCheckAction       | `Functional`          | *undefined*    | Check action        |
| listFilter       | Array          | *undefined*    | List filter key mapping via filter dynamic        |
| showFilter       | boolean          | false    | Show Filter action        |
| sortPositionName       | string          | 'desc'    | Key of sort        |
| typeSort       | string          | 'sortField'    | Type of sort key        |

**HOW TO USE**

![How to use table](/assets/images/use-table.png)

## Animated Numbers
---
Animated random number code is a type of code that generates and displays a random number in an animated fashion

|      Properties       |              Type              |    Default Value     | Description                                                                                                                                                                                                                                                                                               |
| :-------------: | :----------------------------: | :------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| animateToNumber |             number             |      none      | Number to be animated                                                                                                                                                                                                                                                                                     |
|    fontStyle    |      React.CSSProperties?      |      none      | Style of number text                                                                                                                                                                                                                                                                                      |
|  includeComma   |            boolean?            |     false      | Whether the number contains commas                                                                                                                                                                                                                                                                        |
| locale          |           string?              |    en-US       | Formats animated number as per locale. Also it should be used with `inculdeComma` prop. For list of locales, search for "BCP 47 language tags"   |
|   configs(1)    |        SpringConfig[]?         | config.default | This module is using [react-spring](https://www.react-spring.io) and you can refer to this [config option](https://react-spring.io/common/configs). If you pass multiple settings, an animation is randomly assigned to each number. _ DO NOT USE `duration` because of a bug that hasn't been fixed yet_ |
|   configs(2)    | (number, number): SpringConfig | none | The first parameter gives information about the number to be changed, And the second parameter gives information about the order of the changing numbers. You can use that information to adjust the animation by returning the config                                                                    |


## Breadcrumb
Breadcrumb code is a type of markup that helps users navigate through a website. It consists of a list of links that show the user's current location within the site hierarchy.

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| title                     | string     | *undefined*    | Title of breadcrumb        |
| subtitle                     | string     | *undefined*    | Text below title        |
| items                     | Array      | *undefined*    | List breadcrumb        |
| children                     | `ReactNode`      | *undefined*    | React Node children inside breadcrumb       |

**HOW TO USE**

![How to use Breadcrumb](/assets/images/use-breadcrumb.png)

## Ckeditor
Creating custom components for [CKEditor 5](https://ckeditor.com/docs/ckeditor5/latest/features/document-outline.html) involves extending the editor's core functionality and user interface with new elements and interactions. This process requires a deep understanding of the editor's architecture, including its plugin system, data model, and event handling mechanisms.

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| value                     | string     | *undefined*    | Value of editor        |
| field                     | string     | *undefined*    | Key of field       |
| onChange                     | `Functional`      | *undefined*    | Handle change event editor        |
| isReadOnly                     | boolean      | *undefined*    | Readonly mode       |

**HOW TO USE**
Use these components inside the form item antd.

## ErrorBoundary
---
Error boundaries are a React feature introduced in version 16 that allows you to catch and handle JavaScript errors in child components and prevent them from crashing the entire application. They provide a way to display a fallback UI or log the error instead of letting the error bubble up and crash the app.
When there is an error, display the error components defined before.

**HOW TO USE**
```bash
<ErrorBoundary>...</ErrorBoundary>
```

## Input Code
---
This components via [React Ace](https://www.npmjs.com/package/react-ace)

## Konva Editor
---
[React Konva](https://konvajs.org/docs/react/index.html) is a JavaScript library for drawing complex canvas graphics using React. It provides declarative and reactive bindings to the Konva Framework, making it easy to create and manage rich canvas-based applications with React.

### Editor
---
This component is used to build a template of an invitation letter.

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| value                     | string     | *undefined*    | Value of editor        |
| templateImg                     | string     | *undefined*    | Config template Image       |
| backgroundImg                     | strinh      | *undefined*    | Background of letter        |
| onChangeTemplateImg                     | `Functional`      | *undefined*    | Handle change config template images       |
| onChange                     | `Functional`      | *undefined*    | Handle change config template       |

![Toolbar Config](/assets/images/konva-toolbar.png)

Handle some action of Konva via toolbar custom action follow in code:
```bash
 const HeaderToolBar = () => (
    <div className="containerToolbar containerCanvas__header">
      <div className="containerIconeToolbar" onClick={desfazer}>
        <img className="img" src={Desfazer} title="Trở về"></img>
      </div>
      <div className="containerIconeToolbar" onClick={refazer}>
        <img className="img" src={Refazer} title="Kế tiếp"></img>
      </div>
      <div className="containerIconeToolbar">
        <BackgroundChange onChange={(img) => onBackgroundChange(img)}>
          <img className="img" src={BgImage} title="Đổi nền" />
        </BackgroundChange>
      </div>
      <div className="containerIconeToolbar">
        <ImageChange onChange={(img) => loadImage(img)}>
          <img className="img" src={AddImage} title="Thêm ảnh" />
        </ImageChange>
      </div>
      <div className="containerIconeToolbar" onClick={() => loadImage(DEFAULT_QRCODE_IMG_LINK)}>
        <img className="img" src={QrCode} title="QRCode"></img>
      </div>
      <div className="containerIconeToolbar" onClick={() => loadImage(DEFAULT_AVATAR_IMG_LINK)}>
        <img className="img" src={Avatar} title="Avatar"></img>
      </div>
      <div className="containerIconeToolbar" onClick={addNewCircle}>
        <img className="img" src={Circle} title="Khối tròn"></img>
      </div>
      <div className="containerIconeToolbar" onClick={addNewSquare}>
        <img className="img" src={Rectangle} title="Khối vuông"></img>
      </div>
      <div className="containerIconeToolbar" onClick={addNewTriangle}>
        <img className="img" src={Triangule} title="Khối tam giác"></img>
      </div>
      <div className="containerIconeToolbar" onClick={addNewText}>
        <img className="img" src={InsertText} title="Thêm văn bản"></img>
      </div>
      <div className="containerIconeToolbar">
        <Dropdown
          menu={{
            items,
          }}
          trigger={['click']}
          bordered={false}
        >
          <a onClick={(e) => e.preventDefault()}>
            <Space>
              {t('Konva:add_dynamic')}
              <DownOutlined />
            </Space>
          </a>
        </Dropdown>
      </div>

      {arrayObjectsLayer[indexTextSelected] &&
        arrayObjectsLayer[indexTextSelected]?.type === 'text' && (
          <div className="containerIconeToolbar">
            <div className="containerOpcao">
              <select
                disabled={!arrayObjectsLayer[indexTextSelected]}
                value={arrayObjectsLayer[indexTextSelected].fontSize}
                onChange={changeFontSize}
                style={{ width: 120 }}
              >
                {[...new Array(100)].map(
                  (i, index) =>
                    index > 5 && (
                      <option
                        key={index}
                        onClick={() => changeFontSize(`${index * zoom}px`)}
                        value={index}
                      >
                        {`${index}px`}
                      </option>
                    ),
                )}
              </select>
            </div>
          </div>
        )}

      {arrayObjectsLayer[indexTextSelected] &&
        arrayObjectsLayer[indexTextSelected]?.type === 'text' && (
          <div className="list-align">
            <div
              className={classNames({
                'align-item': true,
                active: arrayObjectsLayer[indexTextSelected]?.align === 'left',
              })}
              onClick={() => onChangeAlign('left')}
            >
              <img className="img" src={AlignLeft} title="Căn trái"></img>
            </div>
            <div
              className={classNames({
                'align-item': true,
                active: arrayObjectsLayer[indexTextSelected]?.align === 'center',
              })}
              onClick={() => onChangeAlign('center')}
            >
              <img className="img" src={AlignCenter} title="Căn giữa"></img>
            </div>
            <div
              className={classNames({
                'align-item': true,
                active: arrayObjectsLayer[indexTextSelected]?.align === 'right',
              })}
              onClick={() => onChangeAlign('right')}
            >
              <img className="img" src={AlignRight} title="Căn phải"></img>
            </div>
          </div>
        )}

      {arrayObjectsLayer[indexTextSelected] &&
        arrayObjectsLayer[indexTextSelected]?.type === 'text' && (
          <div className="containerIconeToolbar">
            <div className="containerOpcao">
              <SelectFont
                disabled={!arrayObjectsLayer[indexTextSelected]}
                value={arrayObjectsLayer[indexTextSelected].fontFamily}
                onChange={changeFontFamily}
                style={{ width: 120 }}
              />{' '}
            </div>
          </div>
        )}

      {arrayObjectsLayer[indexTextSelected] &&
        arrayObjectsLayer[indexTextSelected]?.type === 'text' && (
          <div
            className="containerIconeToolbar"
            onClick={() =>
              changeStyle(
                arrayObjectsLayer[indexTextSelected] &&
                  arrayObjectsLayer[indexTextSelected].fontStyle === 'bold'
                  ? 'normal'
                  : 'bold',
              )
            }
            style={
              arrayObjectsLayer[indexTextSelected] &&
              arrayObjectsLayer[indexTextSelected].fontStyle === 'bold'
                ? { backgroundColor: 'grey' }
                : {}
            }
          >
            <img className="img" src={Bold} title="In đậm"></img>
          </div>
        )}
      {arrayObjectsLayer[indexTextSelected] &&
        arrayObjectsLayer[indexTextSelected]?.type === 'text' && (
          <div
            className="containerIconeToolbar"
            onClick={() =>
              changeStyle(
                arrayObjectsLayer[indexTextSelected] &&
                  arrayObjectsLayer[indexTextSelected].fontStyle === 'italic'
                  ? 'normal'
                  : 'italic',
              )
            }
            style={
              arrayObjectsLayer[indexTextSelected] &&
              arrayObjectsLayer[indexTextSelected].fontStyle === 'italic'
                ? { backgroundColor: 'grey' }
                : {}
            }
          >
            <img className="img" src={Italic} title="In nghiêng"></img>
          </div>
        )}
      {arrayObjectsLayer[indexTextSelected] &&
        arrayObjectsLayer[indexTextSelected]?.type === 'text' && (
          <div
            className="containerIconeToolbar"
            onClick={() =>
              setUnderline(
                arrayObjectsLayer[indexTextSelected] &&
                  arrayObjectsLayer[indexTextSelected].textDecoration === 'underline'
                  ? ''
                  : 'underline',
              )
            }
            style={
              arrayObjectsLayer[indexTextSelected] &&
              arrayObjectsLayer[indexTextSelected].textDecoration === 'underline'
                ? { backgroundColor: 'grey' }
                : {}
            }
          >
            <img className="img" src={Underline} title="Gạch dưới"></img>
          </div>
        )}
      {arrayObjectsLayer[indexTextSelected] &&
        arrayObjectsLayer[indexTextSelected]?.type === 'image' && (
          <InputNumber
            value={parseInt(arrayObjectsLayer[indexTextSelected]?.radius)}
            prefix={<RadiusIco />}
            onPressEnter={(e) => onChangeRadius(parseInt(e.target.value))}
            bordered={false}
            controls={false}
          />
        )}

      <div
        className="containerIconeToolbar"
        onClick={tooglePallet}
        style={showPallet ? { backgroundColor: 'grey' } : {}}
      >
        <img className="img" src={FillColor} title="Màu nền"></img>
      </div>
      <div className="containerIconeToolbar" onClick={duplicarObject}>
        <img className="img" src={Duplicate} title="Nhân bản"></img>
      </div>
      <div className="containerIconeToolbar" onClick={() => zommStage(zoom + 1)}>
        <img className="img" src={ZoomOut} title="Zoom -"></img>
      </div>
      <div className="containerIconeToolbar" onClick={() => zommStage(zoom - 1)}>
        <img className="img" src={ZoomIn} title="Zoom +"></img>
      </div>
      <div className="containerIconeToolbar" onClick={() => trazerItem(true)}>
        <img className="img" src={Front} title="Lên trên"></img>
      </div>
      <div className="containerIconeToolbar" onClick={() => trazerItem()}>
        <img className="img" src={Back} title="Sau cùng"></img>
      </div>
      <div className="containerIconeToolbar" onClick={() => backgroundToogle()}>
        <img
          className="img"
          src={BackgroundIcon}
          title="Nền"
          style={!backgroundOn ? { backgroundColor: 'grey' } : {}}
        ></img>
      </div>

      {!!selectedObject && (
        <div className="containerIconeToolbar" onClick={() => deleteSelected()}>
          <img className="img" src={Delete} title="Xóa"></img>
        </div>
      )}
    </div>
  );
  ```
Handle body of Konva via [React Konva](https://konvajs.org/api/Konva.html)

### Render Editor
---
This component is used to render the template that was built by Konva Editor.
Same editor. However, turn off all editor actions.

**HOW TO USE**
Editor used inside Form Item Antd
```bash
    <KonvaEditor
    backgroundImg={backgroundImg}
    onBackgroundChange={(src) => {
      form.setFieldValue({ invitationPhoto: src });
      setBackgroundImg(src);
    }}
    onChange={(tem) => {
      form.setFieldsValue({ template: tem });
      setTemplate(tem);
    }}
    templateImg={templateImg}
    onChangeTemplateImg={(imgArr) => {
      form.setFieldsValue({ templateImg: imgArr });
      setTemplateImg(imgArr);
    }}
  />;
```

To Render, replace all dynamic options by key like:
![Render Image](/assets/images/konva-render.png)

## Modal Preview
---
This code will create a popup window that can render either HTML content or an image letter. The user can switch between the two options using the type in poperties.

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| type                     | 'html' or 'konva'     | `html`    | Type of modal       |
| data                     | string or object     | *undefined*    | Data of render value       |

**HOW TO USE**
```bash
<ModalPreview type="html" data={formData?.inviteEmailTemplate} />
```

## Modal PIN
---
This code will create a popup window that can required PIN code for module Lucky Draw or Check In Out

Two action: confirm actions or get actions
`confirm actions`: To defined action and confirm this via index.js
`get action`: Confirm and then get type of action via get-action.js

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| visible                     | boolean     | false    | Show or hidden popup       |
| setVisible                     | `Functional`     | *undefined*    | Handle show popup       |
| api                     | `Functional`     | *undefined*    | Api to confirm       |
| onClose                     | `Functional`     | *undefined*    | Action after close       |
| action                     | 'lucky-draw' or 'checkin'     | *undefined*    | Action confirm       |
| eventId                     | number     | *undefined*    | Id of event       |

**HOW TO USE**
```bash
   <ModalPin
        visible={visiblePin}
        setVisible={setVisiblePin}
        onClose={onClosePin}
        api={confirmPinCode}
        eventId={userData?.eventId}
        setPinCode={setPinCode}
        action="check-inout"
      />
```

## Select DatePicker
---
This components fork via [react-dropdown-date](https://www.npmjs.com/package/react-dropdown-date) and with Form Item Antd

## Select Font
---
Import some font from Google and select to use this by array was defined.

Import via google fonts
```bash
    <link
      href="https://fonts.googleapis.com/css?family=Abel|Abril+Fatface|Acme|Alegreya|Alegreya+Sans|Anton|Archivo|Archivo+Black|Archivo+Narrow|Arimo|Arvo|Asap|Asap+Condensed|Bitter|Bowlby+One+SC|Bree+Serif|Cabin|Cairo|Catamaran|Crete+Round|Crimson+Text|Cuprum|Dancing+Script|Dosis|Droid+Sans|Droid+Serif|EB+Garamond|Exo|Exo+2|Faustina|Fira+Sans|Fjalla+One|Francois+One|Gloria+Hallelujah|Hind|Inconsolata|Indie+Flower|Josefin+Sans|Julee|Karla|Lato|Libre+Baskerville|Libre+Franklin|Lobster|Lora|Mada|Manuale|Maven+Pro|Merriweather|Merriweather+Sans|Montserrat|Montserrat+Subrayada|Mukta+Vaani|Muli|Noto+Sans|Noto+Serif|Nunito|Open+Sans|Open+Sans+Condensed:300|Oswald|Oxygen|PT+Sans|PT+Sans+Caption|PT+Sans+Narrow|PT+Serif|Pacifico|Passion+One|Pathway+Gothic+One|Play|Playfair+Display|Poppins|Questrial|Quicksand|Raleway|Roboto|Roboto+Condensed|Roboto+Mono|Roboto+Slab|Ropa+Sans|Rubik|Saira|Saira+Condensed|Saira+Extra+Condensed|Saira+Semi+Condensed|Sedgwick+Ave|Sedgwick+Ave+Display|Shadows+Into+Light|Signika|Slabo+27px|Source+Code+Pro|Source+Sans+Pro|Spectral|Titillium+Web|Ubuntu|Ubuntu+Condensed|Varela+Round|Vollkorn|Work+Sans|Yanone+Kaffeesatz|Zilla+Slab|Zilla+Slab+Highlight"
      rel="stylesheet"
    />
    ```


## Show More
---
To show more or less of content or html content

| Properties              | Types           | Default Value  | Description  |
| --- |---| ---| ---|
| content                     | string     | *undefined*    | Value of contents       |
| html                     | string     | *undefined*    | Value of html content       |
| style                     | object     | *undefined*    | style for component       |
| width                     | number     | *undefined*    | Max width content       |
| className                     | string     | *undefined*    | Class name content      |

**HOW TO USE**
```bash
<ShowMore content={content} />
```

## Spin & Spinner
---
This components to define Spin loading animation
**HOW TO USE**
```bash
<Spin/>
```

## Upload Image
---