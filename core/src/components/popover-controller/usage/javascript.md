```javascript
async function presentPopover() {
  const popoverController = document.querySelector('ion-popover-controller');
  await popoverController.componentOnReady();

  const popoverElement = await popoverController.create({
    component: 'profile-page',
    ev: event
  });
  return await popoverElement.present();
}
```
