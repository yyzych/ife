/*
 * 查看review结果并记录。
 *
 * @ques：疑问
 * @mark：标记
 * @ych：这段注释是我添加的。行注释末尾添加括号；段注释前不需要括号
 */

@mark:

@mark: 可以显示的添加转义字符，即使原字符不需要被转义
@mark: \xnn: 表示匹配一个16进数字，nn指定的ASCII字符。如\x43匹配大写的C
@mark: 具体的效果实现和业务逻辑分开
@mark: 正则中的\s匹配几乎所有空白符，但是低版本下 \s 等价于 [ \f\n\r\t\v]。 所以为了兼容，还要加上中文空格 和 &nbsp; 。其中\u3000: 中文空格（全角）的unicode字符表示 (@ych)
@mark: 操作符优先级。typeof > && > ?: