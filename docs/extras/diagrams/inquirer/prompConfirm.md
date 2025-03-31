```javascript
export const promptConfirm = async (
  metadata: UserInputMetadataConfirm
): Promise<boolean> => {
  const { confirm } =
    (await inquirer.prompt) <
    { confirm: boolean } >
    {
      name: "confirm",
      type: "confirm",
      message: metadata.message,
      default: metadata.confirm,
    };
  return confirm;
};
```
