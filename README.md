# Материалы курса

## Настройка окружения

### Ubuntu

```sh
apt update
apt install clang-format gcc gdb make nasm
```

### Docker

Если у вас возникли проблемы с настройкой окружения, вы можете воспользоваться
уже готовым окружением, в котором доступны все необходимые инструменты, при
помощи [Docker](https://docs.docker.com/desktop/setup/install/linux/)

```sh
# в директории, куда склонирован репозиторий задачи
docker run --rm -ti -w /sandbox -v $PWD:/sandbox ghcr.io/nsu-syspro-llp/runner
```

### NixOS

Необходимое окружение описано в этом файле [shell.nix](./shell.nix)

## Linux

- [Справочник по системным вызовам ядра Linux](https://www.chromium.org/chromium-os/developer-library/reference/linux-constants/syscalls/)

## x86-64

- [Соглашение о вызовах](https://stackoverflow.com/a/2538212)
- [Справочник инструкций](https://www.felixcloutier.com/x86/)
- [System V ABI](https://gitlab.com/x86-psABIs/x86-64-ABI/-/jobs/artifacts/master/raw/x86-64-ABI/abi.pdf?job=build)

## Aarch64

- [Соглашение о вызовах](./arm64_docs/procedure_call_standard.pdf)
- [Справочник инструкций (A-profile)](./arm64_docs/a64_isa_a_profile.pdf)
- [System V ABI](./arm64_docs/system_v_abi.pdf)
