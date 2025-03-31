```javascript
export const promptList = async (
    metadata: UserInputMetadataList,
): Promise<string> => {
    const availableValues = getValueFromChoiceOps(metadata.list);
    const { list } = await inquirer.prompt<{
        list: (typeof availableValues)[number];
    }>({
        name: 'list',
        type: 'list',
        message: metadata.message,
        choices: metadata.list,
        default: metadata.value,
    });
    return list;
};
```
