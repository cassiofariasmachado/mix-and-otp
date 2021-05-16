# KvUmbrella

## Tests

* Running normal tests execute `mix test`
* Running distributed tests execute:

```powershell
# Start bar node (on apps/kv folder)
iex.bat --sname bar -S mix

# Run tests (on kv_umblela folder)
elixir --sname foo -S mix test --only distributed
```

## Releases

Releases configuration is under project definition in `mix.exs`.

### Creating an release

* Set `MIX_ENV=prod`
* For create foo release run `mix release foo`
* For create bar release run `mix release bar`
