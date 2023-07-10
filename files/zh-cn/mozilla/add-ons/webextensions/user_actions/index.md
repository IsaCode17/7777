---
title: �û�����
slug: Mozilla/Add-ons/WebExtensions/User_actions
---

{{AddonSidebar}}

һЩ WebExtension API ִ�еĹ���ͨ���������û�������ִ�еġ����磺

- ���е������ڵ���������������û�����ʱ��ʾ�������ڣ�������һ�� {{WebExtAPIRef("browserAction.openPopup")}} API ������չ�����Ա�̷�ʽ�򿪵������ڡ�
- �����չ��������˲�������û�ͨ��ͨ����������õ��û������ĳЩ���֣����硰��ͼ/��������˵���������������һ�� {{WebExtAPIRef("sidebarAction.open")}} API ������չ�����Ա�̷�ʽ����������

Ϊ����ѭ��û�����⡱��ԭ������ API ֻ�ܴ��û������Ĵ�������ڲ����á��û����������������ݣ�

- �����չ����������������ҳ�������
- ѡ����չ����������Ĳ˵��
- ������չ����ļ��̿�ݼ������� Firefox 63 ��ʼ������Ϊ�û���������
- �������չ����������һ���ҳ���еİ�ť��

���磺

```js
function handleClick() {
  browser.sidebarAction.open();
}

browser.browserAction.onClicked.addListener(handleClick);
```

ע�⣬��ͨ��ҳ�е��û�����������Ϊ���ڴ�Ŀ�ĵ��û����������磬����û�������ͨ��ҳ�еİ�ť���������ݽű���Ϊ�ð�ť��ӵ���Ĵ�����򣬲����ڸô������������չ����ĺ�̨ҳ�淢����Ϣ����ô��̨ҳ�����Ϣ������򲻱���Ϊ�����û�������

���⣬����û�����Ĵ������ȴ� [promise](/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)����ô����Ϊ�û����봦������״̬���ᶪʧ�����磺

```js
async function handleClick() {
  let result = await someAsyncFunction();

  // this will fail, because the handler lost its "user action handler" status
  browser.sidebarAction.open();
}

browser.browserAction.onClicked.addListener(handleClick);
```
