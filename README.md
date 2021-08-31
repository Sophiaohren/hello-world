
curl --proto '=https' --tlsv1.2 -sSL https://sh.getsynth.com | sh
mkdir synth_workspace && cd synth_workspace && synth init
mkdir my_namespace

{
    "type": "array",
    "length": {
        "type": "number",
        "subtype": "u64",
        "constant": 1
    },
   "content": {
        "type": "string",
        "pattern": "Hello world!"
    }
}

synth generate my_namespace/
