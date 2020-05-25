# sys-fonts
Install custom fonts for all users (system wide).

Example Playbook
----------------

    - hosts: server
      
      vars:
        # -- custom - fonts_repository --
        fonts_repository:
          - { name: 'MyriadPRO-BLACK (OpenType)', file: 'MyriadPro-Black.otf', url: 'http://{{ def_ans_rep }}/resources/veg/fonts/MyriadPro/MyriadPro-Black.otf'}
          - { name: 'MyriadPro-BlackIt (OpenType)', file: 'MyriadPro-BlackIt.otf', url: 'http://{{ def_ans_rep }}/resources/veg/fonts/MyriadPro/MyriadPro-BlackIt.otf'}
          - { name: 'MyriadPro-Bold (OpenType)', file: 'MyriadPro-Bold.otf', url: 'http://{{ def_ans_rep }}/resources/veg/fonts/MyriadPro/MyriadPro-Bold.otf'}

      roles:
        - sys-custom-fonts

