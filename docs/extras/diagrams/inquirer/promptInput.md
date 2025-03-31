```javascript
export const promptInput = async (
    metadata: UserInputMetadataInput,
): Promise<string> => {
    const { input } = await inquirer.prompt<{
        input: string;
    }>({
        name: 'input',
        type: 'input',
        message: metadata.message,
        default: metadata.input,
        transformer: (input: string) => input.trim(),
    });
    return input;
};
```
