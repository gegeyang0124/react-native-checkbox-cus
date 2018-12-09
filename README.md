# react-native-checkbox-cus
勾选框

### 安装
npm i --save react-native-checkbox-cus

### 展示
<p>
    <img src ="./showImg/chk.jpg" 
          height="auto" width="400" />
</p>

### 使用
```javascript
import CheckBox from "react-native-checkbox-cus";

<CheckBox
    style={{flex: 1, padding: 10}}
    onClick={(isChecked)=>{

    }}
    leftText={"CheckBox"}
/>

 <CheckBox
            style={{flex: 1, padding: 10}}
            onClick={(isChecked)=>{
                 this.setState({
                     isChecked:!isChecked
                 })
               }}
            isChecked={this.state.isChecked}
            checkedImage={<Image source={require('../../page/my/img/ic_check_box.png')} style={this.props.theme.styles.tabBarSelectedIcon}/>}
            unCheckedImage={<Image source={require('../../page/my/img/ic_check_box_outline_blank.png')} style={this.props.theme.styles.tabBarSelectedIcon}/>}
        />
```

### API


属性              | 类型     | 可选 | 默认值     | 描述
----------------- | -------- | -------- | ----------- | -----------
style  | ViewPropTypes.style  | true |   |   Custom style checkbox
leftText | PropTypes.string |true |   | Custom left Text
leftTextStyle  |  Text.propTypes.style | true |  | Custom left Text style
rightText | PropTypes.string |true |   | Custom right Text
rightTextView | PropTypes.element | true |   | Custom right TextView
rightTextStyle  | Text.propTypes.style | true |  | Custom right Text style
checkedImage  |  PropTypes.element  | true  | Default image | Custom  checked Image
unCheckedImage  |  PropTypes.element  | true  |  Default image  | Custom  unchecked Image
isChecked  |  PropTypes.bool |  false  |  false  | checkbox checked state
onClick   |  PropTypes.func.isRequired |  false  |  | callback  function
disabled  |  PropTypes.bool            | true  |  false | Disable the checkbox button
checkBoxColor | PropTypes.string | true |   | Tint color of the checkbox image (this props is for both checked and unchecked state)
checkedCheckBoxColor | PropTypes.string | true |   | Tint color of the checked state checkbox image (this prop will override value of `checkBoxColor` for checked state)
uncheckedCheckBoxColor | PropTypes.string | true |   | Tint color of the unchecked state checkbox image (this prop will override value of `checkBoxColor` for unchecked state)
imageStyle | PropTypes.style | true |   |  Custom checkbox image style


### 欢迎交流
欢迎提问交流；若有bug，请添加bug截图或代码片段，以便更快更好的解决问题。<br>
欢迎大家一起交流

### [我的博客](http://blog.sina.com.cn/s/articlelist_6078695441_0_1.html)
