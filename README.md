# 设置Element UI的Message消息提示每次只弹出一个

### Element的Message提示是点击一次触发一次的。要是一直点，会一直弹出，影响体验。

### 新建resetMessage.js

### 在main.js引入
```
import resetMessage from '@/components/common/resetMessage';
Vue.prototype.$message = resetMessage;
```

### 使用
```
this.$message.success('成功提示');
this.$message.error('失败提示');
```

