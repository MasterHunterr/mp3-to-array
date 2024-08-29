def file_to_c_array(filename, array_name):
    with open(filename, 'rb') as f:
        byte_array = f.read()

    array_str = ', '.join(f'0x{byte:02x}' for byte in byte_array)
    array_length = len(byte_array)

    c_array = f"unsigned char {array_name}[] = {{\n    {array_str}\n}};\n"
    c_array += f"unsigned int {array_name}_size = {array_length};\n"

    output_filename = f"{array_name}.h"
    with open(output_filename, 'w') as f:
        f.write(c_array)

    print(f"array saved to {output_filename}")

# Example usage
file_to_c_array('game_over.mp3', 'game_over_mp3_bin')
