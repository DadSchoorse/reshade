reshade_src = [
    'source/effect_codegen_spirv.cpp',
    'source/effect_expression.cpp',
    'source/effect_lexer.cpp',
    'source/effect_parser.cpp',
    'source/effect_preprocessor.cpp',
    'source/effect_symbol_table.cpp',
]

reshade_lib = static_library('reshade', reshade_src,
    include_directories : [ vkBasalt_include_path, './deps/spirv/include/spirv/unified1', './source'])

reshade_dep = declare_dependency(
    link_with : [ reshade_lib ])