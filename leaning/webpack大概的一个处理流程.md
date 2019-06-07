st=>start: 注册印象笔记
a=>condition: 是否已经购买马克飞象
b1=>operation: 您已购买马克飞象可以使用markdown语法
c=>end: 欢迎使用马克飞象
b2=>operation: 还未能成功购买马克飞象但你可以免费试用10天
d=>condition: 是否要购买马克飞象
e1=>operation: 您已成功购买马克飞象欢迎使用
e2=>operation: 试用10天后将会到期欢迎购买

st->a
a(yes)->b1->c
a(no)->b2->d
d(yes)->e1->c
d(no)->e2
