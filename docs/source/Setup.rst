Local Development Setup
======================

This guide explains how to set up the PrepPal application locally for development and testing.

Prerequisites
-------------
* `Node.js 16+ <https://nodejs.org/en>`_ (LTS version recommended)
* `Git <https://git-scm.com/>`_
* Terminal/shell access

Cloning the Repository
----------------------

1. Open your terminal
2. Navigate to your preferred development directory
3. Run the clone command:

.. code-block:: bash

   git clone https://github.com/yourusername/preppal.git
   cd preppal

Installation
------------

1. Install project dependencies:

.. code-block:: bash

   npm install

   # or if using yarn
   yarn install

2. Configure environment variables (if needed):
   - Copy `.env.example` to `.env`
   - Update with your local values

Running the Application
----------------------

Start the development server:

.. code-block:: bash

   npm start

This will:
- Start the application
- Open browser automatically (typically at http://localhost:3000)
- Enable hot reloading for development

Testing
-------

Run the test suite with:

.. code-block:: bash

   npm test

Additional Commands
------------------

.. list-table:: Useful NPM Scripts
   :widths: 30 70
   :header-rows: 1

   * - Command
     - Purpose
   * - ``npm run build``
     - Create production build
   * - ``npm run lint``
     - Run code linter
   * - ``npm run format``
     - Format code automatically
   * - ``npm run storybook``
     - Launch UI component browser

Troubleshooting
--------------

Common Issues
~~~~~~~~~~~~~

**Node.js version mismatch**
.. code-block:: bash

   nvm use  # if using Node Version Manager

**Missing dependencies**
.. code-block:: bash

   rm -rf node_modules package-lock.json
   npm install

**Port already in use**
.. code-block:: bash

   sudo lsof -i :3000  # find process
   kill -9 <PID>       # replace <PID> with actual process ID

Getting Help
------------
* Check the ``README.md`` for project-specific notes

