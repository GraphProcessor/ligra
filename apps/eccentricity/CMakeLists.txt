foreach (exec_file kBFS-1Phase-Ecc kBFS-Ecc FM-Ecc LogLog-Ecc kBFS-Exact RV CLRSTV TK Simple-Approx-Ecc)
    add_executable(${exec_file} ${exec_file}.C)
    target_include_directories(${exec_file} PUBLIC "../../ligra")
endforeach ()
